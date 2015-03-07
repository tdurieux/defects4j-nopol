# Chart - Nopol angelic condition repair


- Nb patch found: 6/25

| #Bug | Nb Statements Analyzed | Nb Angelic Value Found | Exec. time | Patch Found |
|------|---------------|--------------|------------|------------|
| 1 |  464 |  0 |  288896ms | NO |
| 2 |  166 |  0 |  98484ms | NO |
| 3 | NONE | NONE | > 6h | NO |
| 4 | NONE | NONE | > 6h | NO |
| 5 |  3 |  1 |  101534ms | YES |
| 6 | NONE | NONE | > 6h | NO |
| 7 |  122 |  0 |  82130ms | NO |
| 8 | IGNORED | IGNORED | IGNORED | IGNORED |
| 9 |  8 |  1 |  102417ms | YES |
| 10 |  2 |  0 |  68609ms | NO |
| 11 |  19 |  0 |  74732ms | NO |
| 12 |  339 |  0 |  156112ms | NO |
| 13 |  38 |  1 |  112855ms | YES |
| 14 |  361 |  0 |  226535ms | NO |
| 15 |  878 |  1 |  278129ms | NO |
| 16 |  45 |  0 |  74080ms | NO |
| 17 |  1 |  1 |  100162ms | YES |
| 18 |  95 |  0 |  79762ms | NO |
| 19 |  512 |  0 |  220260ms | NO |
| 20 |  35 |  0 |  70404ms | NO |
| 21 |  11 |  1 |  101755ms | YES |
| 22 |  97 |  0 |  77493ms | NO |
| 23 |  218 |  0 |  114512ms | NO |
| 24 |  11 |  0 |  65026ms | NO |
| 25 |  8 |  1 |  98569ms | YES |
| 26 | NONE | NONE | > 6h | NO |
## Patches

### Bug 5

```
----INFORMATION----
Nb Statements Analyzed : 3
Nb Statements with Angelic Value Found : 1
Nopol Execution time : 101534ms
----PATCH FOUND----
org.jfree.data.xy.XYSeries:561: CONDITIONAL !(org.jfree.data.xy.XYSeries.this.allowDuplicateXValues)
```
### Bug 9

```
----INFORMATION----
Nb Statements Analyzed : 8
Nb Statements with Angelic Value Found : 1
Nopol Execution time : 102417ms
----PATCH FOUND----
org.jfree.data.time.TimeSeries:935: CONDITIONAL ((org.jfree.data.time.TimeSeries.DEFAULT_RANGE_DESCRIPTION.length())==(startIndex))||((!((startIndex)!=(1)))&&(start!=null))
```
### Bug 13

```
----INFORMATION----
Nb Statements Analyzed : 38
Nb Statements with Angelic Value Found : 1
Nopol Execution time : 112855ms
----PATCH FOUND----
org.jfree.chart.block.BorderArrangement:482: CONDITIONAL null!=null
```
### Bug 17

```
----INFORMATION----
Nb Statements Analyzed : 1
Nb Statements with Angelic Value Found : 1
Nopol Execution time : 100162ms
----PATCH FOUND----
org.jfree.data.time.TimeSeries:880: PRECONDITION (1)==(start)
```
### Bug 21

```
----INFORMATION----
Nb Statements Analyzed : 11
Nb Statements with Angelic Value Found : 1
Nopol Execution time : 101755ms
----PATCH FOUND----
org.jfree.data.Range:335: PRECONDITION (((1)+(1))<((org.jfree.data.Range.this.upper)-(org.jfree.data.Range.this.lower)))||(!(((1)+(1))<=(org.jfree.data.Range.this.lower)))
```
### Bug 25

```
----INFORMATION----
Nb Statements Analyzed : 8
Nb Statements with Angelic Value Found : 1
Nopol Execution time : 98569ms
----PATCH FOUND----
org.jfree.data.statistics.DefaultStatisticalCategoryDataset:110: CONDITIONAL ((org.jfree.data.statistics.DefaultStatisticalCategoryDataset.this.maximumRangeValue)<(org.jfree.data.statistics.DefaultStatisticalCategoryDataset.this.maximumRangeValueIncStdDev))&&(!((org.jfree.data.statistics.DefaultStatisticalCategoryDataset.this.maximumRangeValue)<=(1)))
```