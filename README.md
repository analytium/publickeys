# publickeys
Analytium Engineers' SSH public keys

This is an authoritative source of the SSH public keys for Analytium engineers.

If you wish to grant access via SSH you can obtain the public key for the relevant engineer. Each key is named as the email address of the owner.

To ensure the integrity of these keys the following workflow is enforced:

1. No direct commits can be made to main. Each new key is submitted via a branch.
2. After submitting a Pull Request, the commit must be reviewed by two different members of staff before it can be merged.
3. The commit history is retained, providing an audit trail of changes and approvers.

# Key Management
Should any corresponding private keys need to be revoked due to loss of control or compromise, the public key will be replaced **and** a note added to this README with details.

Regular rotation of private/public pairs will just show as an updated public key file.

We would always recommend that you remove the public key from your system when access is no longer required, and retrieve the latest key the next time access is granted.

# Analytium How-To
1. Pull the repo to ensure you are in sync: git pull
2. Create a new branch for your key: git checkout -b **branch-name**
3. Add your file as *first*.*last*@analytium.co.uk.pub and add to git: git add .
4. Commit your staged change: git commit -m 'addition of *mykey*'
5. Push your branch: git push
6. Submit a Pull Request on github.com/analytium/publickeys
