# RouteScanAuto 路径漏洞探测工具
![RouteScanAuto](https://img.shields.io/badge/RouteScanAuto-blue.svg)

**RouteScanAuto** 是一款用于扫描网站路径漏洞的自动化工具，通过分析给定的 URL 或 URL 列表，帮助安全研究人员检测网站中的常见漏洞路径，提升网站安全性。

## 💡主要功能
- 扫描单个 URL 或从文件中读取多个 URL 进行扫描。
- 支持 URL 爬取并与漏洞扫描结合，自动化检测潜在的安全漏洞。
- 扫描结果可以输出到指定文件，方便后续分析。

## 📌参数说明
| 参数        | 描述                                                        |
| ----------- | ----------------------------------------------------------- |
| `-u`        | 单个 URL，用于扫描的单个网站地址（如 `http://example.com`）。    |
| `-f`        | 包含多个 URL 的文件路径，每行一个 URL，支持批量扫描。        |
| `-tt`       | 用于 URL 爬取，指定 `js.exe` 的 `-t` 参数值。例如，`-tt 1` 会运行 `js.exe -t 1`。不需要 URL 爬取时可忽略此参数。 |
| `-output`   | 扫描结果保存的文件，默认为 `results.txt`，你可以指定一个自定义文件名。 |

## 🚀使用示例
示例 1：扫描单个 URL
扫描单个网站 URL：
RouteScanAuto.exe -u http://example.com

示例 2：扫描多个 URL
从文件中读取多个 URL，进行批量扫描：
RouteScanAuto.exe -f urls.txt

示例 3：开启 URL 爬取功能
开启 URL 爬取功能并指定爬取深度：
RouteScanAuto.exe -u http://example.com -tt 1

✅联动工具https://github.com/kk12-30/JSFinder-go

示例 4：保存扫描结果到指定文件
将扫描结果保存到 scan_results.txt：
RouteScanAuto.exe -u http://example.com -output scan_results.txt



