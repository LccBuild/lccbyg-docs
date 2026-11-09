---
layout: lccbyghelp40
title: "Open Source Licencer"
date: "2024-01-01"
search: false
---

OBS: Se også "Vilkår for brug af beregningsprogrammet LCCbyg"

LCCbyg 4.4 bygger på .NET, .NET MAUI, Blazor, Windows App SDK og WebView2 fra Microsoft og benytter bl.a. følgende eksterne biblioteker. Listen viser de biblioteker, LCCbyg bruger direkte, samt de vigtigste af dem, de selv bygger på.

## Programbiblioteker

 | Bibliotek                                  | Version         | Licens                    | Licenstekst                                                                  |
 | ------------------------------------------ | --------------- | ------------------------- | ---------------------------------------------------------------------------- |
 | BlazorSortableList                         | 2.1.2           | MIT                       | https://www.nuget.org/packages/BlazorSortableList/2.1.2/License              |
 | CodeBeam.MudBlazor.Extensions              | 9.1.0           | MIT                       | https://licenses.nuget.org/MIT                                               |
 | CommunityToolkit.Maui                      | 15.0.1          | MIT                       | https://licenses.nuget.org/MIT                                               |
 | Csv                                        | 2.0.245         | MIT                       | https://licenses.nuget.org/MIT                                               |
 | CsvHelper                                  | 33.1.0          | MS-PL OR Apache-2.0       | https://licenses.nuget.org/MS-PL%20OR%20Apache-2.0                           |
 | FluentValidation                           | 12.1.1          | Apache-2.0                | https://licenses.nuget.org/Apache-2.0                                        |
 | FuzzySharp                                 | 2.0.2           | MIT                       | https://licenses.nuget.org/MIT                                               |
 | Humanizer                                  | 3.0.10          | MIT                       | https://licenses.nuget.org/MIT                                               |
 | Markdig                                    | 1.3.2           | BSD-2-Clause              | https://licenses.nuget.org/BSD-2-Clause                                      |
 | Math-Expression-Evaluator                  | 1.4.0           | Apache-2.0                | https://licenses.nuget.org/Apache-2.0                                        |
 | Microsoft.ML.OnnxRuntime                   | 1.29.0          | MIT                       | https://www.nuget.org/packages/Microsoft.ML.OnnxRuntime/1.29.0/License       |
 | Microsoft.ML.Tokenizers                    | 2.0.0           | MIT                       | https://licenses.nuget.org/MIT                                               |
 | MudBlazor                                  | 9.9.0           | MIT                       | https://licenses.nuget.org/MIT                                               |
 | MudBlazor.Markdown                         | 9.0.0           | MIT                       | https://licenses.nuget.org/MIT                                               |
 | NPOI                                       | 2.8.0           | Apache-2.0                | https://www.nuget.org/packages/NPOI/2.8.0/License                            |
 | PSC.Blazor.Components.MarkdownEditor       | 10.0.9          | MIT                       | https://licenses.nuget.org/MIT                                               |
 | ReverseMarkdown                            | 6.2.1           | MIT                       | https://licenses.nuget.org/MIT                                               |
 | Svg.Skia                                   | 5.2.2           | MIT                       | https://licenses.nuget.org/MIT                                               |
 | Toolbelt.Blazor.HotKeys2                   | 6.2.1           | MPL-2.0                   | https://licenses.nuget.org/MPL-2.0                                           |

## Biblioteker, de ovenstående bygger på

 | Bibliotek                                  | Version         | Licens                    | Licenstekst                                                                  |
 | ------------------------------------------ | --------------- | ------------------------- | ---------------------------------------------------------------------------- |
 | AngleSharp                                 | 1.5.2           | MIT                       | https://licenses.nuget.org/MIT                                               |
 | BouncyCastle.Cryptography                  | 2.6.2           | MIT                       | https://licenses.nuget.org/MIT                                               |
 | Enums.NET                                  | 5.0.0           | MIT                       | https://licenses.nuget.org/MIT                                               |
 | ExCSS                                      | 4.3.1           | MIT                       | https://licenses.nuget.org/MIT                                               |
 | ExtendedNumerics.BigDecimal                | 2025.1001.2.129 | MIT                       | https://licenses.nuget.org/MIT                                               |
 | Google.Protobuf                            | 3.30.2          | BSD-3-Clause              | https://licenses.nuget.org/BSD-3-Clause                                      |
 | HarfBuzzSharp                              | 14.2.0          | MIT                       | https://licenses.nuget.org/MIT                                               |
 | MathNet.Numerics.Signed                    | 5.0.0           | MIT                       | https://licenses.nuget.org/MIT                                               |
 | SharpZipLib                                | 1.4.2           | MIT                       | https://licenses.nuget.org/MIT                                               |
 | SkiaSharp                                  | 4.148.0         | MIT                       | https://licenses.nuget.org/MIT                                               |
 | Svg.Custom                                 | 5.2.2           | MS-PL                     | https://licenses.nuget.org/MS-PL                                             |
 | ZString                                    | 2.6.0           | MIT                       | https://licenses.nuget.org/MIT                                               |

## Grafer og søgemodel

 | Komponent                                  | Version         | Licens                    | Licenstekst                                                                  |
 | ------------------------------------------ | --------------- | ------------------------- | ---------------------------------------------------------------------------- |
 | Apache ECharts (grafer)                    | 6.1.0           | Apache-2.0                | https://github.com/apache/echarts/blob/master/LICENSE                        |
 | MiniLM-L6-danish-encoder-v2 (søgemodel)    | v2              | MIT                       | https://huggingface.co/KennethTM/MiniLM-L6-danish-encoder-v2                 |

Søgemodellen bygger på sentence-transformers/all-MiniLM-L6-v2 og kører lokalt i LCCbyg.
