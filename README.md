# ledger-board

## Project Goals

I am creating this application as a practice project to learn more about
- big data
- neural networks
- web frameworks

## Project Statement

This project aims to build a web app visualizer for personal finance data, saved in [Ledger](https://github.com/ledger/ledger) format. The application will use **neural networks** to predict the next transactions. The application will use the following technologies:
- backend: python (Django)
- frontend: Angular
- database: Redis
- big data management: Spark, kafka,
- some kind of linter
- structured logging: sentry, jsonlogs
- unit tests
- deploy with [kubernetes](https://github.com/kubernetes/kubernetes)
- fully github workflow with issues, roadmap and milestones

## Developement

We strongly encourage to use Nix to have a consistant developement environment across devices. You can enter the developement environmenti with the following command:
```bash
nix develop
```

If you don't have nix, you nee to have `python3` and you need to install all the dependencies. You can use the command:
```bash
pip install -r requirements.txt
```

### Running the project

You can run the backend with the following command:
```bash
cd backend
python3 manage.py runserver 
```
You can run the frontend with the following command, assuming you have installed the modules via `npm i`:
```bash
cd frontend
npx ng serve --open
```
