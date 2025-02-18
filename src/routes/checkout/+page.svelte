<script>
    // This is your test secret API key.
    const stripe = require('stripe')('sk_test_51QtfbbKuJCFFLFjtNZiROvDtGFA3FxncJSsP7ATwGQiwJhrNWRpo3r52a334VeUFgtfUF27Yagr28LNc3wXWkecw000zYyNSb3');
    const express = require('express');
    const app = express();
    app.use(express.static('public'));

    app.post('/create-checkout-session', async (req, res) => {
    const session = await stripe.checkout.sessions.create({
        line_items: [
        {
            // Provide the exact Price ID (for example, pr_1234) of the product you want to sell
            price: '{{PRICE_ID}}',
            quantity: 1,
        },
        ],
        mode: 'payment',
        success_url: `/success`,
        cancel_url: `/cancel`,
    });

    res.redirect(303, session.url);
    });

    app.listen(4242, () => console.log('Running on port 4242'));
</script>
<section>
    <div class="product">
    <img src="https://i.imgur.com/EHyR2nP.png" alt="The cover of Stubborn Attachments" />
    <div class="description">
        <h3>Stubborn Attachments</h3>
        <h5>$20.00</h5>
    </div>
    </div>
    <form action="/create-checkout-session" method="POST">
    <button type="submit" id="checkout-button">Checkout</button>
    </form>
</section>