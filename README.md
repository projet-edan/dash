Edan Core staging tree 0.16
===========================



https://www.projetedan.org


What is Edan?
-------------

Edan, a user-focused cryptocurrency, which you can spend anywhere, anytime and anytime what amount for charges less than 1 cent.
The users may decide to take advantage of optional privacy offers by Edan. Edan uses Proof of Service (PoSe) and Proof of Work (PoW) to secure his blockchain. 
Proof of work is provided by minors, while proofs of service are provided by masternodes, where some people are ready to implant a certain amount of Edan in the network to show their commitment to the network and specific tasks.

For more information, as well as an immediately useable, binary version of
the Dash Core software, see https://www.projetedan.org/get-edan/.

Feature
-------------------
PrivateSend is a payment anonymization service. Similar to cryptocurrency tumblers, it uses a coin shuffle strategy to keep transactions anonymous and untraceable. Each payment is passed through masternodes in a few rounds of mixing. Since each participant in the mixing session only signs their transaction entry, it is impossible to know where the money is going. Once all participants have signed their entries, they are sent to the network. The mixing process can be repeated up to eight times. The more mixing cycles there are, the more difficult it is to track the original shipper of parts.

InstantSend is an instant transactions service. A transaction is verified by consensus of randomly selected masternodes. Then it is added to the next block. As a result, masternodes guarantee near instant confirmation of transactions, so there is no need to wait for standard block confirmations. Similar to PrivateSend, masternodes charge fees for instant confirmation of transactions.

The Decentralized Autonomous Organization (DAO) is a network service which allows all members of the community to make proposals for network development and to vote. The DAO is funded by block rewards: periodically generated superblocks provide a higher percentage of the reward to the DAO. So, in a way, DAO turns the Edan network into a kind of self-regulating entity.

Edan masternodes provide proof of service and additional network security. They run all of the services mentioned above and are enticed to do so by the block rewards they receive alongside miners.

Sporks are a mechanism to safely deploy and activate new functionality after updating the node software. This mechanism was first implemented by Dash. Sporks are used to ensure simultaneous updates of the entire network so that the new logic is applied correctly. Sporks are activated with a special service message broadcast from one of the developer addresses across the network. Self-regulation, anonymity, fast payments, masternode services and the spork mechanism make Edan one of the best blockchains. However, there is one feature that may scare some users off - the Proof of Work consensus algorithm. While consensus is implemented more efficiently in Dash than in Bitcoin, it still consumes a lot of time and energy.

License
-------

Dash Core is released under the terms of the MIT license. See [COPYING](COPYING) for more
information or see https://opensource.org/licenses/MIT.

Development Process
-------------------

The `master` branch is meant to be stable. Development is normally done in separate branches.
[Tags](https://github.com/dashpay/dash/tags) are created to indicate new official,
stable release versions of Dash Core.

The contribution workflow is described in [CONTRIBUTING.md](CONTRIBUTING.md).

Testing
-------

Testing and code review is the bottleneck for development; we get more pull
requests than we can review and test on short notice. Please be patient and help out by testing
other people's pull requests, and remember this is a security-critical project where any mistake might cost people
lots of money.

### Automated Testing

Developers are strongly encouraged to write [unit tests](src/test/README.md) for new code, and to
submit new unit tests for old code. Unit tests can be compiled and run
(assuming they weren't disabled in configure) with: `make check`. Further details on running
and extending unit tests can be found in [/src/test/README.md](/src/test/README.md).

There are also [regression and integration tests](/test), written
in Python, that are run automatically on the build server.
These tests can be run (if the [test dependencies](/test) are installed) with: `test/functional/test_runner.py`

The Travis CI system makes sure that every pull request is built for Windows, Linux, and OS X, and that unit/sanity tests are run automatically.

### Manual Quality Assurance (QA) Testing

Changes should be tested by somebody other than the developer who wrote the
code. This is especially important for large or high-risk changes. It is useful
to add a test plan to the pull request description if testing the changes is
not straightforward.

Translations
------------

Changes to translations as well as new translations can be submitted to
[Dash Core's Transifex page](https://www.transifex.com/projects/p/dash/).

Translations are periodically pulled from Transifex and merged into the git repository. See the
[translation process](doc/translation_process.md) for details on how this works.

**Important**: We do not accept translation changes as GitHub pull requests because the next
pull from Transifex would automatically overwrite them again.

Translators should also follow the [forum](https://www.dash.org/forum/topic/dash-worldwide-collaboration.88/).
