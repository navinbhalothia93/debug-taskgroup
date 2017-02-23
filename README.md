# RISC-V Debug task group

The RISC-V Debug Task Group was established to propose specifications for debug on RISC-V implementations. The scope of the group includes run-control and trace debug, but the current focus is to agree upon a standard for run-control debug.

The group is chaired by Tim Newsome (SiFive Inc).

The best way to get involved in this effort is to join and participate in the [RISC-V debug mailing list](https://groups.google.com/a/groups.riscv.org/forum/#!forum/debug).

## Run-control debug

Run-control debug allows you to halt, step, resume, to set breakpoints, and to access GPRs+CSRs+memory. There have been two main proposals for run-control, and much of the group's time has been spent understanding the differences and trade-offs between these two approaches, with the goal of producing a single unified specification.

### Key documents and proposed specifications

* The ['Instruction' design](https://dev.sifive.com/documentation/risc-v-external-debug-support/).
* The ['Direct' design](https://groups.google.com/a/groups.riscv.org/d/msg/debug/N2Qu17lALe4/4lzibYmvCQAJ). The primary author of this proposal has also started work on [a version that hopes to combine the best of both proposals](https://groups.google.com/a/groups.riscv.org/d/msg/debug/HYCuX8oP6Ew/NLTr1IWNBAAJ).
* Tim Newsome's [comparison between the two approaches](https://sifive.github.io/debug-mechanism-comparison/).
* Stefan Wallentowitz and Alex Bradbury produced a [presentation](https://goo.gl/9abgZa) aiming to summarise proposals so far, briefly survey what other architectures do for run-control debug, and propose a path towards a unified specification. They went on to give a more detailed [proposal](https://goo.gl/Uy5V2k) for an approach with a base memory map, with optional instruction feeding.
* The options for interfaces were [put to a vote](https://sifive.github.io/debug-mechanism-comparison/poll), which [resulted](https://sifive.github.io/debug-mechanism-comparison/poll-results/results.html) in the decision to [pursue a spec with a unified abstract interface](https://groups.google.com/a/groups.riscv.org/d/msg/debug/FDmZUk7YCNw/e9e5pN3mCQAJ). Once the costs of translating from the abstract interface to instruction feeding are better understood, the group may agree that providing two optional interfaces is preferable.

## Meetings

In addition to discussions on the mailing list, the group has recently started a series of meetings.

### Upcoming

 * Wednesday 1st March, 2017. 8am PST.

### Previous

  * 22nd February, 2017. [Slides](https://docs.google.com/presentation/d/1LKeLg7Lw-O-yd6-K0Q0NauUyyK-fee7aRHeY2uh-neU/edit?usp=sharing). [Notes](https://groups.google.com/a/groups.riscv.org/d/msg/debug/ECH84s1E4gM/OKCPxVRwAwAJ).
  * 15th February, 2017. [Slides](https://docs.google.com/presentation/d/15PabK0Lj6c1ASlhs88yAd598BN3NhCHRnzBbQZEr4Gs/edit?usp=sharing). [Notes](https://groups.google.com/a/groups.riscv.org/d/msg/debug/ZH5Z0YSDvtg/xgjRyMZNAQAJ).
  * 8th Februrary, 2017. [Slides](https://docs.google.com/presentation/d/15PabK0Lj6c1ASlhs88yAd598BN3NhCHRnzBbQZEr4Gs/edit?usp=sharing). [Notes](https://groups.google.com/a/groups.riscv.org/d/msg/debug/bMbG1KESEnk/khvNcHe0DwAJ).
  * 1st February, 2017. [Slides](https://docs.google.com/presentation/d/1npb-thIWwbQP9IAiRNDmzmMoWOBgm5Tyo283zlDXQkg/edit?usp=sharing). [Notes](https://groups.google.com/a/groups.riscv.org/d/msg/debug/KU22vtt_pWI/QuBoiXWMDQAJ).
  * 25th January, 2017. [Slides](https://docs.google.com/presentation/d/1TApV32HsTzilEqZO6FfWQcCo-zHJxl3IZlR0CJ47Jec/edit?usp=sharing). [Notes](https://groups.google.com/a/groups.riscv.org/d/msg/debug/FgOOnKQW8TY/jnhOLJNqCwAJ).
  * 18th January, 2017. [Slides](https://docs.google.com/presentation/d/1dSBiJQSRdUdpEPW_eS_gTWC6viaz3lIrFHe1j2lwGQ8/edit?usp=sharing). [Notes](https://groups.google.com/a/groups.riscv.org/d/msg/debug/9-k_39cb5xo/uMp_25lECQAJ).
  * 11th January, 2017. [Slides](https://docs.google.com/presentation/d/1p2ny3cb2fjTeADlgy1Q4fhlY5pCmsO4LmLvNZ6ha8-A/edit?usp=sharing). [Notes](https://groups.google.com/a/groups.riscv.org/d/msg/debug/oFfmIQgkb_k/xq6faXkSFAAJ).
  * 5th January, 2017. [Slides](https://docs.google.com/presentation/d/1GlQNnZmCJ0sVICde6IOnv3bBvPYkHsU0AiAElGFyxNw/edit?usp=sharing). [Notes](https://groups.google.com/a/groups.riscv.org/d/msg/debug/r4jt2VmWXpI/7ktkIF46EgAJ).
  * 21st December, 2016. [Slides](https://docs.google.com/presentation/d/1Aikb1R2xposb9no0f3AQq-2FCC9zX9m2MyBBQBZcgDc/edit?usp=sharing). [Notes](https://groups.google.com/a/groups.riscv.org/d/msg/debug/LqaZtesnqUg/QlM0i3HxDQAJ).
  * 15th December, 2016. [Slides](https://docs.google.com/presentation/d/1QnTYCawE_wbeU_F6c0F0QoUA6sKHf4fvcyrlK0Nz0KY/edit?usp=sharing). [Notes](https://groups.google.com/a/groups.riscv.org/d/msg/debug/37AFJNRdkME/r_Z4bbO_BgAJ).
  * 7th December, 2016. [Slides](https://docs.google.com/presentation/d/1zMAUUgEf1nydUpKVB5Tg9cdOJrl4M0pWdTgHoMEVD4Q/edit?usp=sharing). [Notes](https://groups.google.com/a/groups.riscv.org/d/msg/debug/qoYAY36-5HQ/o6DSzDXlBAAJ).
  * 30th November, 2016. [Slides](https://docs.google.com/presentation/d/1jOjG20-gwtcGybZg2Bu3StV6ljZZV9n2SQAEjKWQwDE/edit?usp=sharing). [Notes](https://groups.google.com/a/groups.riscv.org/d/msg/debug/ucaYL8pNfxo/Rv81fi6nCwAJ).
