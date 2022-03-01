# phd-thesis-latex

Provides a package `mitchell-thesis.sty`, which can be used by downloading the file and placing it next to your `main.tex` document. 
From there just `usepackage{mitchell-thesis}` as usual. 
The package takes one optional argument, `fancy`, which enables blue coloring of hyperlinks and sectioning numbers, and modifies the font of chapter/section/subsection/subsubsection titles.

The package makes some assumptions about font.
It uses the `notomath` package, which enables the Noto font for serif, sans-serif, math, etc.
This has the benefit that the Noto font includes Greek characters (enabled with the command `\notoseriflgr`).
Using LGR mode, I defined nice-looking upright symbols for microns (μ) and sigma (σ).
Using these, I defined a few units, e.g., `\uWpercubicm`, which prints the units for microwatts per cubic meter.
If a different font is enabled after importing this package, these commands won't work anymore.

The following commands are provided. These can be used as templates to create similar commands that utilize Noto font capabilities.

| Command          |  Function   |
|------------------|-------------|
|`\labelphantom`   |  Allows creating subfigure labels out of a single `\includegraphics` command                                                   |
|`\muser`          |  Upright μ, serif                                                                                                              |
|`\sigmaser`       |  Upright σ, serif                                                                                                              |
|`\hrow`           |  Creates a single-column, two-row table cell with text centered horizontally and vertically                                    |
|`\largegraphics`  |  Allows graphics to take up 6.5 inches of page width, running past narrower margins. Drop-in replacement for `\includegraphics`|
|`\midtilde`       |  Creates a nice looking `~` with the Noto font. Just calls `\textasciitilde`. Other fonts may require changing this command.   |
|`\uWpercubicm`    |  Prints unit for microwatts per cubic meter                                                                                    |
|`\mWpersquarem`   |  Prints unit for milliwats per square meter                                                                                    |
|`\um`             |  Prints unit for micrometers                                                                                                   |
|`\kgpercubicm`    |  Prints unit for kilograms per cubic meter                                                                                     |
|`\JperK`          |  Prints unit for Joules per Kelvin                                                                                             |
|`\WpermperK`      |  Prints unit for Watts per meter per Kelvin                                                                                    |
|`\kmsquare`       |  Prints unit for kilometers squared                                                                                            |
|`\kmcubed`        |  Prints unit for kilometers cubed                                                                                              |
|`\persec`         |  Prints unit for 1/second                                                                                                      |
|`\degCperkm`      |  Prints units for degrees Celsius per kilometer                                                                                |
|`\degCperMa`      |  Prints units for degrees Celsius per Ma                                                                                       |
|`\degC`           |  Prints degrees Celsius                                                                                                        |
|`\kmperMa`        |  Prints units for kilometers per Ma                                                                                            |
|`\mmperyr`        |  Prints units for millimeters per year                                                                                         |
|`\cmperyr`        |  Prints units for centimeters per year                                                                                         |
|`\atomic{238}{U}` |  Given a number and a symbol, formats an element properly                                                                      |
|`\ArAr`           |  Prints the correct formatting for 40Ar/39Ar                                                                                   |
|`\PbU`            |  Prints the correct formatting for 206Pb/238U                                                                                  |
|`\PbPb`           |  Prints the correct formatting for 206Pb/207Pb                                                                                 |
|`\RayleighTaylor` |  Ensures consistent formatting, `Rayleigh--Taylor`                                                                             |
|`\RT`             |  Ensures consistent formatting, `R--T`                                                                                         |
