# Proposal

This pallet allows the Community to signal its sentiment on-chain . A Proposal can be used to change the value of the settings of a Community.

For example, a community member could propose to change the languages spoken and get buy-in from the rest of the community. A Proposal is structured as follows:

| Proposal Component | Description                                                                                                                              |
| ------------------ | ---------------------------------------------------------------------------------------------------------------------------------------- |
| community          | The Community to which the Proposal belongs                                                                                              |
| proposal           | The content of the proposal                                                                                                              |
| options            | A list of choices that the community members can choose from to express their opinion                                                    |
| historical         | A flag to highlight if a Proposal is an important event for the Community (e.g. voting the removal of a language from its official list) |

In the first version of this pallet no deadlines are attached to a proposal so that this will be an “on-going” sentiment from the community for a specific topic. A simple majority is considered in terms of signaling a sentiment. Members cannot cast multiple votes.

Community and Proposals are in a one to many relationship meaning that one Community can have multiple Proposals but one Proposal belongs to one specific Community.

<figure><img src="https://lh6.googleusercontent.com/Xq9X8K8IqvyQiOJIVPOs2IBxcKPB2yn-szAXNSO_iLz0ef7agkxRdlZbVN_pk60tLuQqmr9fhaDBrPYF_7736h-D_wRqj-Rs7J-hMhJ1hgFe8Dgi81Zo4upYQt45mtn24EDFoZ5mNdTE0NMDhdTM-TQUGkp_WyPCS0iv_Z1wRie3Q8eA_yHLNZ9tSTWOyA" alt=""><figcaption></figcaption></figure>

The following version of the Proposal pallet will allow values of the Community to be changed through community governance and deadlines to be configured so that voting will be bound to a specific epoch instead of being ongoing. Communities will be free to disable this setting if they wish instead to keep the sentiment as an ongoing on-chain expression of their stance.
