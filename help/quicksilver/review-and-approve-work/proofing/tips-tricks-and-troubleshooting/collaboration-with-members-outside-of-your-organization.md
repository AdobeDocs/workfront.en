

# Proofing collaboration limitations with people outside of your organization

There are some limitations to be aware of when communicating with people outside of your organization when they are added to a proof, specifically if the person outside of your organization has proofing access in a separate environment.

## Contacts with the distinction of Member

There are three types of contacts that exist in a proofing environment:

* **Users**: Users have a Workfront Proof login in your organization's environment.
* **Members**: Members have their own Workfront Proof login in another organization's environment(not your own). You cannot convert members to users in your environment.
* **Guests**: Guests do not have their own Workfront Proof login in your organization's environment, but you have added their details to your account (for example, guest reviewers on proofs). You can convert guests to users.

Because Members can't be converted to users, their ability to tag people in proof comments is limited to users from *their original organization*.

**Example:** Company A invites an outside user to review a proof. This user already exists in separate proof environment, Company B.

&nbsp;

When Company A invites the outside user to the proof, the outside user is added to Company A's contact list as a Member. Reviewers in the proof workflowm from Company A can tag the outside user in proof comments because they are now in the contact directory of Company A.

&nbsp;

The outside user cannot tag users from Company A, even though they are on the same proof workflow, because the users from Company A have not been added as contacts to Company B.

&nbsp;

The outside user from Company B can tag other users from Company B if they are on the proof workflow or if they have permission to share the proof with new users because those users exists as contacts in Company B. 
