# Datathon template

I made this template for the datathon. It has a Next.js dashboard, a Python API built with FastAPI, and a PostgreSQL database on AWS. The database uses Amazon Aurora PostgreSQL and stores user accounts, sessions, and portfolio holdings.

I forked [Studio Admin](https://github.com/arhamkhnz/next-shadcn-admin-dashboard) for the frontend. You can sign in, add stocks to your portfolio, and open a stock to see its price chart and related news. On Home, the Discover table shows which S&P 500 stocks appeared in the most articles over the past 24 hours. Click your name in the sidebar to open settings.

The backend gets stock prices from Yahoo Finance through the Python library yfinance. For news, it makes HTTP requests to the API behind [StocksFeed](https://stocksfeed.benollomo.com/), an earlier project of mine.

## Run it locally

Start the [FastAPI server](backend-server/README.md) in one terminal, then follow the [dashboard setup](frontend-dashboard/README.md) in another. Open [the dashboard](http://localhost:3000) and sign in or create an account.
