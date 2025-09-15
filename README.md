# EventHub – Fil Rouge DevOps

EventHub is a web-based event management and ticketing application.
This repository will serve as a guide throughout the **DevOps** journey.

---


## Git Workflow

- **main** : The main branch, the cleanest one (production)
- **dev** : The most updated branch
- **feature/*** : Development branches for each new feature

Contributions are made via Pull Requests to `dev`.


## Commit Conventions

We use the [Conventional Commits] convention (https://www.conventionalcommits.org).

### Format :
`<type>(scope?): <description>`

### Main types :

- `feat` : adding a feature
- `fix` : bug fix
- `docs` : documentation
- `style` : formatting (indentation, spaces, etc...)
- `test` : adding or modifying tests

Examples :
- `feat(auth): added JWT connection`
- `fix(api): fix error 500 on GET /events`
- `docs(readme): added commit conventions`


## Git Hooks

Hooks will be implemented with **Husky** and **lint-staged** to automate checks:
- `pre-commit`: checks the lint and formatting of the code
- `commit-msg`: Checks that messages comply with **Conventional Commits**


## Next steps
- Setting up the Docker environment (backend + frontend + DB)
- Added first tests and CI/CD pipeline
