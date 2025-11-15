AgriTrace DAO is a blockchain-based system that records agricultural crop batches on Algorand.
It provides transparent and verifiable data for farmers, distributors, and consumers.

Setup & Installation

Clone the repository

Install dependencies

Start Algorand LocalNet

Deploy the smart contract

Run backend and frontend

Smart Contract

The smart contract stores batch details such as batch ID, farmer name, crop type, location, and harvest date.
Code is available in /backend/contract/smart_contract.py.



Architecture

– Smart contract stores data on-chain
– Backend connects to Algorand and runs LoRa verification
– Frontend allows users to register and view batches

LoRa Testing

Transaction IDs were verified on LoRa App Lab to confirm on-chain data accuracy.

Deployment

Frontend deployment link will be added after hosting.
# React + Vite

This template provides a minimal setup to get React working in Vite with HMR and some ESLint rules.

Currently, two official plugins are available:

- [@vitejs/plugin-react](https://github.com/vitejs/vite-plugin-react/blob/main/packages/plugin-react) uses [Babel](https://babeljs.io/) (or [oxc](https://oxc.rs) when used in [rolldown-vite](https://vite.dev/guide/rolldown)) for Fast Refresh
- [@vitejs/plugin-react-swc](https://github.com/vitejs/vite-plugin-react/blob/main/packages/plugin-react-swc) uses [SWC](https://swc.rs/) for Fast Refresh

## React Compiler

The React Compiler is not enabled on this template because of its impact on dev & build performances. To add it, see [this documentation](https://react.dev/learn/react-compiler/installation).

## Expanding the ESLint configuration

If you are developing a production application, we recommend using TypeScript with type-aware lint rules enabled. Check out the [TS template](https://github.com/vitejs/vite/tree/main/packages/create-vite/template-react-ts) for information on how to integrate TypeScript and [`typescript-eslint`](https://typescript-eslint.io) in your project.
