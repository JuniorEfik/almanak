# Almanak Platform Getting Started Guide

This guide will walk you through setting up and deploying your first strategy on the Almanak platform.

## Prerequisites

- Python 3.7 or higher
- A wallet with at least $5 USD worth of ETH on your chosen network
- Access to the Almanak platform dashboard

## Step 1: Install the Almanak SDK

First, install the Almanak SDK, which provides all the tools you need to create and manage your strategies.

```bash
pip install almanak
```

## Step 2: Authorize the SDK with the Platform

Next, authorize your local SDK to communicate with the Almanak platform.

```bash
almanak auth
```

This will open a browser window where you can generate an API key, which you can paste into the terminal.

## Step 3: Create a Template Strategy

You can create a new strategy using one of the available templates. The template provides a starting point for you to customize for your specific needs.

```bash
almanak strat new
```

This will create a new directory with the strategy code and configuration files. The template includes comments explaining each component and how to customize it.

## Step 4: Create a New Strategy Repository

1. In the UI, under **Strategies**, click on the **Create Strategy** button
2. Give it a name and description
3. Copy the resulting `push` command

## Step 5: Push Your Strategy to the Platform

Once you've customized your strategy, push it to the Almanak platform where it can be executed by a Deployment.

Paste the `push` command from the UI into your terminal.

## Step 6: Create a Wallet

Now that your strategy is on the platform, you need to create a wallet for your Deployment to use.

1. Navigate to the **Wallets** section in the Almanak dashboard
2. Click **Create Wallet**
3. Give it a name and select the network where you want to deploy your wallet. Choose the network that you have at least $5 USD worth of ETH on
4. Review the wallet creation details and click **Confirm**
5. Sign the three transactions that are generated in your wallet. For more information on what these transactions do, see the Wallets page

> **Note:** The wallet creation process may take a few minutes to complete as the necessary smart contracts are deployed.

## Step 7: Add Gas for Your Wallet

Your Deployment needs gas to execute transactions on the blockchain. Let's add some gas to your wallet.

1. In the **Wallets** section, find your newly created wallet
2. Find the **Wallet Gas** section and click **Top Up**
3. Enter the amount of ETH you want to add for gas. For this tutorial, we'll add $2 USD worth of ETH
4. Complete the transaction from your personal wallet

## Step 8: Add Funds to Your Wallet

Now, add the funds that your strategy will manage.

1. Still in the **Wallets** section, click on the **Deposit** button
2. Select the token you want to add
3. Enter the amount. For this tutorial, we'll add $2 USD worth of ETH
4. Complete the transaction from your personal wallet

## Step 9: Connect Your Telegram Account (Optional)

You can connect your Telegram account to your Almanak account to receive notifications on your Telegram account when your Deployment is executing a transaction.

1. Go to the **Settings** section in the dashboard
2. Click **Notifications**
3. Follow the instructions to connect your Telegram account

## Step 10: Start Your Deployment!

Finally, let's start your Deployment and watch your strategy in action.

1. Go to the **Deployments** section in the dashboard
2. Click **Create Deployment**
3. Select your strategy from the dropdown
4. Select your newly created wallet
5. Configure any strategy-specific parameters
6. Click **Create Deployment**
7. Confirm the permission settings

Your Deployment is now live and will begin executing your strategy according to its programming. You can monitor its performance in the **Deployments** dashboard, which provides real-time updates on transactions, performance metrics, and any issues that might arise.

## Support

For additional help and documentation, visit the [Almanak Documentation](https://docs.almanak.co/docs/getting-started/) or contact support through the platform dashboard.

## License

This project is licensed under the MIT License - see the LICENSE file for details.
