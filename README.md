## What is Local-Initia?

Local-Initia is a complete Initia testnet and ecosystem containerized with Docker and orchestrated with a simple `docker-compose` file. It is designed to be a sandbox for developers to learn about and build on Initia.

Local-Initia comes preconfigured with opinionated, sensible defaults for standard testing environments. If other projects mention testing on Local-Initia, they are referring to the settings defined in this repo.

Local-Initia has the following advantages over a public testnet:

- Easily modifiable world states
- Quick to reset for rapid iterations
- Simple simulations of different scenarios
- Controllable validator behavior

## Prerequisites

- [Docker](https://www.docker.com/)
- [`docker-compose`](https://github.com/docker/compose)

## Install Local-Initia

1. Run the following commands::

```sh
$ git clone --depth 1 https://github.com/initia-labs/local-initia
$ cd local-initia
```

2. Make sure your Docker daemon is running in the background and [`docker-compose`](https://github.com/docker/compose) is installed.

## Start, stop, and reset Local-Initia

- Start Local-Initia:

```sh
$ docker-compose up
```

Stop Local-Initia:

```sh
$ docker-compose stop
```

Reset the world state:

```sh
$ docker-compose rm
```

### Modifying genesis

You can change the `genesis.json` file by altering `config/genesis.json`. To load your changes, restart your Local-Initia.

## Accounts

Local-Initia is pre-configured with one validator and 10 accounts with `uinit` for initia and `umin` for minitia.
Also there are 4 accounts for `executor`, `batch`, `challenger` and `output` for rollup testing.
You can check the account information as follows.

| User       | Address                                    | Key                                                                                                                    |
|------------|--------------------------------------------|------------------------------------------------------------------------------------------------------------------------|
| validator  | init1r8ymvqrayx5evum755nlg6ckpv9q2lphp860v0 | "perfect pyramid knee frown response caution museum feature quiz infant hair design fancy dream fan mixed spider exotic champion child pride grant camera grief" |
| user0      | init1u6tna8tje9h0qenzqd3p2ucteqwcfxwegyy8ag | "earth actor drink pact away alpha unlock card rack avoid evil sail raven outdoor stereo begin hunt pizza hover paddle hair gloom sock educate"                 |
| user1      | init19nn70mhuylm492vdwfxlg69r6wmaptcl5wecvt | "banner december bunker moral nasty glide slow property pen twist doctor exclude novel top material flee appear imitate cat state domain consider then age"    |
| user2      | init1wzenw7r2t2ra39k4l9yqq95pw55ap4sm4vsa9g | "diamond donkey opinion claw cool harbor tree elegant outer mother claw amount message result leave tank plunge harbor garment purity arrest humble figure endless" |
| user3      | init1y60n8pp6hcl4fx0h83n6reqp5k2vr2t87yy3gt | "empower finish monitor prevent grid marble payment viable orphan debris question scare struggle walnut attract vacant artist tell envelope betray tribe planet city noble" |
| user4      | init1dlkwrn0kyjkxnda7fl3svkrmmpeytc8u926l5w | "real magnet congress immense fetch someone sugar kit tail love select ill exit text track jump silver make ghost juice matter dress spirit wait"                 |
| user5      | init1al85pyj5l32eleese6fmrfmn8a7m69hevlkpkx | "teach runway asset able faith tackle topple child picture pelican punch rocket lady wide warm close tail extend note borrow wedding vague cart force"           |
| user6      | init174knscjg688ddtxj8smyjz073r3w5mmsp3m0m2 | "cheap start amused certain dune unique diet enemy surround total grab item reduce engage office brain border liar eagle random unknown avoid chapter report"     |
| user7      | init1l9le0esewecpfs7587jw5tg26t8lzhevacttef | "make drama daughter whisper language proud inmate great edge good piece peace saddle dust pilot mixture identify unfold true first hurry toddler pull reunion"   |
| user8      | init1dc3zgdzmmkdre8nhc9czy2cr62gvpnm83ge07t | "vapor census car shoulder require network entire smooth idle fish reject river yellow excuse animal mention stove summer ramp honey junk recipe abuse body"      |
| user9      | init1gx9jf222pthadx034xf7rz05wzgqakdujlcwap | "debate tent visa mandate clap thumb skirt arrange bean session expand describe intact before elder empty clown route scissors helmet nation language half purse" |
| output     | init1m64l7gj3sr7t67z5ez8q2v5jw5lrjhytmvy8v3 | "airport hidden cake dry bleak alcohol enough tower charge cash modify feature analyst suffer bus oyster initial coffee wine plug paper damp sock afraid"        |
| executor   | init12mx0x0z9hx25dnga59ev76zf89dmlptnkmfer6 | "recycle sight world spoon leopard shine dizzy before public use jungle either arctic detail hawk output option august hedgehog menu keen night work become"    |
| batch      | init1jr737xpgmdd5ucrhh6wh49ewnsx008rsmnhs92 | "broken umbrella tent include pet simple amount renew insect page sound whip shock dynamic deputy left outside churn lounge raise mirror toss annual fat"        |
| challenger | init10hfaydk485frjr207ve4qzyfy4cxz8kcg2cka6 | "purity yard brush wagon note forest athlete seek offer clown surround cover present ski bargain obvious cute admit gloom text shaft super impose rubber"       |
