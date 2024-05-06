
# Subscription Contract

This project provides a smart contract for managing subscriptions on a blockchain using the Soroban SDK.

## Overview

The Subscription Contract allows users to create, renew, and cancel subscriptions for various services on the blockchain. It provides functions to check whether a subscription is active for a given user and service.

## Features

- **Create Subscription**: Users can create new subscriptions for services by specifying the user's address, service ID, and duration of the subscription in seconds.
- **Check Subscription Status**: The contract allows checking whether a subscription is active for a given user and service at any point in time.
- *(Potential)* **Renew Subscription**: Functionality to renew existing subscriptions, extending their duration.
- *(Potential)* **Cancel Subscription**: Capability to cancel active subscriptions before their end time.

## Usage

To use this contract in your Soroban blockchain project, follow these steps:

1. Import the `soroban_sdk` crate into your project.
2. Define your subscription data structure using the `Subscription` struct.
3. Implement the `SubscriptionContract` trait with required contract functions such as `create_subscription` and `is_subscription_active`.
4. Use the `contractimpl!` macro to implement the contract functions.
