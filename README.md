# Java code for "Linearity of a drug response curve observed and explained in a hybrid model for SARS–CoV–2".

The Java file uses and is dependent on the Hybrid Autmata Library (HAL) software package, for more information see https://halloworld.org/.

The main goal of the project is to examine the probability of stochastic infection extinction as a function of the virus removal rate parameter.
There are two main modes of the code: "experimental" and "theoretical".

By using the "experimental" switch, one thousand randomized simulations are executed with the same initial condition. A single infected cell is placed in the geometric center of a 200 x 200 cell grid with zero initial virus concentration. The one infected cell either dies instantly or starts producing virions. The experimental probability of extinction is calculated by counting the number of cases where early infection extinction happens stochastically and at least 99% of the cells remain uninfected.

On the other hand the code also serves as a tool to understand the former PoE by producing data on offspring distribution.
