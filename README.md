# FLoC Simulator

Command line FLoC simulator to calculate CohortID with using host list and cluster data.

## Build
```
$ go get
go: downloading golang.org/x/net v0.0.0-20210405180319-a5a99cb37ef4
$ go build
```
## Example
Input json file of host list for history data is needed to run. See [host_list.json](./host_list.json) file in this repo.

Comuputed result below shows the same cohort Id as Chromium that has the history of servers included in host_list.json.
```
$ ./floc_simulator host_list.json
domain_list: [nikkei.com hatenablog.com nikkansports.com yahoo.co.jp sponichi.co.jp cnn.co.jp floc.glitch.me ohtsu.org]
sim_hash: 779363756518407
cohortId: 21454
```
![](floc_demo_screenshot.png)

## References
- [Federated Learning of Cohorts (FLoC)](https://github.com/WICG/floc)
- [What is Federated Learning of Cohorts (FLoC)?](https://web.dev/floc/)
- [FLoC Origin Trial & Clustering](https://www.chromium.org/Home/chromium-privacy/privacy-sandbox/floc)
- [Evaluation of Cohort Algorithms for the FLoC API](https://github.com/google/ads-privacy/tree/master/proposals/FLoC)
- [Measuring Sensitivity of Cohorts Generated by the FLoC API](https://docs.google.com/viewer?a=v&pid=sites&srcid=Y2hyb21pdW0ub3JnfGRldnxneDo1Mzg4MjYzOWI2MzU2NDgw)
- [Federated Learning Component](https://chromium.googlesource.com/chromium/src/+/refs/heads/main/components/federated_learning/)



