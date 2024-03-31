# Java code for "Linearity of a drug response curve observed and explained in a hybrid model for SARS–CoV–2".

The Java file uses and is dependent on the Hybrid Autmata Library (HAL) software package, for more information see https://halloworld.org/.

The main goal of the project is to examine the probability of stochastic infection extinction as a function of the virus removal rate parameter.
There are two main modes of the code: the variable experimentalOrTheoretical can be set to either "experimental" and "theoretical".

By using the "experimental" switch, one thousand randomized simulations are executed with the same initial condition. A single infected cell is placed in the geometric center of a 200 x 200 cell grid with zero initial virus concentration. The one infected cell either dies instantly or starts producing virions. The experimental probability of extinction is calculated by counting the number of cases where early infection extinction happens and at least 99% of the cells remain uninfected.

The code also serves as a tool to understand the former experimental probability of extinction by producing data on offspring distribution. This mode can be used with the "theoretical" switch. This mode, too, works with 1000 simulations, but here the newly infected cells do not produce virions -- only the single original infected cell does. This way we are able to measure precisely the number of offsprings of the original infected cells. The offspring distribution can be used to explain the results observed for the experimental probability of extinction. For more detail, see the article with the same title.
