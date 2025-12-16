This is a [Next.js](https://nextjs.org) project bootstrapped with [`create-next-app`](https://nextjs.org/docs/app/api-reference/cli/create-next-app).
## Deploy
https://ria-currency-challenge.vercel.app/

## Description
XChange is a currency exchange dashboard that is useful for converting money from one currency to another, viewing different currency exchange rates and more. It uses Frankfurter API for getting the currency conversion rates. It has three principal tools:

1.- Currency Converter: With this tool, you can select a base currency and a target currency, then, enter an amount of money in base currency to convert it to money in target currency.

2.- Exchange Rates table: This tool shows all the current currency exchange rates based on the base currency you previously selected in the Currency Converter.

3.- Exchange Rates graphic (Between base currency and target currency): (I will explain it in the Innovation feature section).

## Setup instructions

First, update sudo, install node and use it:
```bash
sudo apt update
nvm install node
nvm use node
```

Then, install dependencies

```bash
npm install
```

In case of error while doing npm install:
```bash
sudo apt install -y libatomic1
```

For starting the project at localhost:

```bash
npm run dev
```

Open [http://localhost:3000](http://localhost:3000) with your browser to see the result.

## Innovation feature
The feature that I implemented is the Exchange Rates Graphic that I mentioned before, this tool shows how the conversion rates between the base currency and the target currency has varied over time, you can select different date ranges: Last 7 days, Last month and Last year. With this options you can view the variance in conversion from the base currency to the target currency that you selected before in the selected date range. I chose it because it is very useful for people who want to send money internationally, as they can check when their base currency will have the highest value in the destination currency before sending it. This feature greatly improves the user experience, since the visual presentation makes it easier to understand the conversion rates between two currencies.

## AI Usage
In this project I used AI for debugging small functions in different sections and ensure the correct functioning of the app, Also, I asked it for the Graphic's gradient.

## Assumptions and Trade-Offs
The only two assumptions I made were:

1.- The select base currency and select destination currency buttons are general for all of the components, so it does not repeat over the app.
2.- In the Exchange Rates table I directly show the conversion between (1 currency) to Base Currency and not the rates themselves

And the principal trade-off I made is, for changing the base and destination currency in real time, I had to load all of the currency exchange rates again and it is a bit laggy because it changes the Table and the Graphic in real time.

## Possible Improvements
With more time, I would improve the UI, making it prettier and more comfortable for the user experience, also, improve general details like being able to write letters in the conversion input, and improving the responsive design (it is responsive, but it can be better). 


