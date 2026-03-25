# Tagging Strategy - Cloud Engineering Bootcamp

## 1. Required Tags
To ensure 100% cost attribution, every resource must carry these four keys:

| Key | Values | Description |
| :--- | :--- | :--- |
| **Environment** | `production`, `staging`, `development` | Environment type |
| **Owner** | `[team-name]` or `[email]` | Person/Team responsible |
| **Project** | `bootcamp`, `internal-app`, `data-pipeline` | Associated project |
| **CostCenter** | `eng-101`, `mkt-202`, `admin-000` | Financial department code |

## 2. Naming Conventions
* **Keys:** PascalCase (e.g., `CostCenter`)
* **Values:** lowercase-with-dashes (e.g., `platform-team`)

## 3. Enforcement Policy
* **Audit:** AWS Config rule `required-tags` checks compliance every 24 hours.
* **Automation:** Terraform `default_tags` used for all new infrastructure.
