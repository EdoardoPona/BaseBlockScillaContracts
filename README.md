# BaseBlockScillaContracts
This repo contains the smart contracts for the BaseBlock crowdfunding platform. 

The helper contract simulates the users and what happes on the non-blockchain side of the platform (storing users's funds).
This is because the BaseBlock contract assumes that everything else works with zil tokens. The users would pay the platform with
fiat currency, then an exchange would convert it to zil tokens, which would then be stored as XSGD. This is simulated with 
the helper contract. 
BaseBlock is explained by this presentation 
https://docs.google.com/presentation/d/19vYSXcbu7CmkivkuZXuugWxzcrW4bQN3uc_1dDO23Mk/edit?usp=sharing

for each project in the platform we deploy one BaseBlock contract. this handles the milestones and the associated deadlines that 
the project has to complete, and releases the money as time advances,according to the backers' validation of the project's progress.

This makes sure that the projects that sign up, are not frauds, and the money wasted on projects that don't deliver is minimal.
If a project were to stop delivering, the backers would simply vote against the release of it's funds. 
