# Pipeline keywords

| Keyword | Meaning |

| `$default-branch` | Placeholder in GitHub starter templates, replaced with the real branch name (e.g. main) when the workflow is created from the template. If copied by hand, it stays literal and the trigger never fires. |

| `-j0 -p` (gprbuild) | `-j0`: use as many parallel compile processes as CPU cores. `-p`: create missing output folders. A compiler setting, not a GitHub job. |

| `release` trigger | Starts the workflow when a GitHub Release is published. |

| `artifact` | Files a job saves so later jobs or people can use them. Needed because each job runs on a separate machine. |

| `environment` | A named deployment target (dev, test, prod) that can carry rules such as required approvers. |

| `needs` | One job waits for another and only runs if it succeeded. |

| `permissions` | Limits what the workflow's token can do in the repo. Least privilege. |

| `matrix` | One job that runs once per combination of values (e.g. Python versions). |

| `uses` / `run` | `uses` runs a prebuilt action. `run` runs a shell command. |

| `runs-on` | The type of machine the job runs on. |