# Rebase

We should only rebase branches when:

- BETA is out of sync of main

If BETA is out of sync a --force push is required to get out of the "out-of-sync" status
This require that we are able to do a --force on the branch

## Fix a branch out of sync of main
1. git checkout beta
2. git rebase main
3. git add .
4. git rebase --continue
5. git push --origin HEAD --force

__Note:__ Run step 3 and 4 until rebasing is done
