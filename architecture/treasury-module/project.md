# Project

The Project pallet allows any community member to propose an initiative to the Treasury Committee in order to get funding.

A Project is a data structure that holds a promoter, an hashed proposal, amount requested and Milestones.

Each Milestone contains the account responsible for achieving the milestone, the beneficiary of the amount of the Milestone, the amount itself and the Project it refers to.

A constraint is placed to make sure that all the Milestones amounts summed together add up to the total Project’s funding. Each Project needs to have at least one Milestone.

Any Community member is free to propose a Project although following the best practice from the Dotsama [pallet-treasury](https://paritytech.github.io/substrate/master/pallet\_treasury/index.html). Slashing happens any time a proposal is rejected by the Committee. Slashed funds are automatically transferred to the Treasury funds.

<figure><img src="https://lh3.googleusercontent.com/iBUUDXuGdVVyQdzoQXvGcRkk0IxtN1u-aUS4RUxrWkjqdj-6-whJyXJCRg77gQ7NpD6Aq8y2w4Ln3Eq4ZEBAaNrYcV4Cp1WOowNCNsuei3_r9RH8DkxsEmEQUpeA-LS6blHy0DP2D-tnjRWcXVpz4EK2G3H0GHKCI5c9XAXaoYtnhj5H5o0Cpf0dfgsI6w" alt=""><figcaption></figcaption></figure>
