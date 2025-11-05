# Check list

- [ ] Set Actions permissions (_⚙️ Settings > ▶️ Actions > General > Workflow permissions_)
  > <img width="572" height="263" alt="Screenshot 2025-10-16 at 8 33 32 PM" src="https://github.com/user-attachments/assets/48c29bd0-de77-4d8e-84a0-87e9209d35b1" />
  - [ ] Read and write permissions
  - [ ] Allow GitHub Actions to create and approve pull requests
- [ ] Dispatch initialization workflow (_▶️ Actions > Initialization procedure > Run Workflow_)
  - The action will:
    1. Clone a subrepo of the `dist` branch within the `main` branch (so that changes within `./dist` of the `main` branch are automatically synced to the `dist` branch via [.github/workflows/subrepo-push-dist.yml](https://github.com/pmalacho-mit/suede-dependency-template/blob/main/.github/workflows/subrepo-push-dist.yml))
    2. Replaces the content of this README with specifics around installing this repository as a subrepo dependency
    3. Self destruct (meaning it will delete [.github/workflows/initialize.yml](https://github.com/pmalacho-mit/suede-dependency-template/blob/main/.github/workflows/initialize.yml))
  > <img width="1496" height="611" alt="Screenshot 2025-11-04 at 11 38 51 PM" src="https://github.com/user-attachments/assets/a32bcbc7-4ec3-492e-bf7a-1cc86db79f36" />
