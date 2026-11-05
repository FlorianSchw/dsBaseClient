## DataSHIELD argument names

Checked against the naming rules (version 0.1.0).

| Package | Side | Functions | Arguments | Already following the rules |
|---|---|---|---|---|
| dsBase | server | 133 | 455 | 53 % |
| dsBaseClient | client | 118 | 625 | 72 % |

- **302 renames proposed** (69 of them under a rule that is still open), 0 approved, 0 skipped, 0 applied.
- **86 need a decision** (unresolved or conflicting): fill in `proposed` and approve, or skip.
- 0 of the entries were classified by Claude (arguments the code could not place).

## dsBaseClient

### Need a decision

| Function | Current | Proposed | Rule | Confidence | Reason |
|---|---|---|---|---|---|
| `ds.asCharacter` | `x.name` | – | classes | medium | object of unknown class  |
| `ds.asInteger` | `x.name` | – | classes | medium | object of unknown class  |
| `ds.asLogical` | `x.name` | – | classes | medium | object of unknown class  |
| `ds.asNumeric` | `x.name` | – | classes | medium | object of unknown class  |
| `ds.assign` | `toAssign` | – | unresolved | low | role unknown  |
| `ds.Boole` | `Boolean.operator` | – | unresolved | low | role unknown  |
| `ds.changeRefGroup` | `ref` | – | unresolved | low | role unknown  |
| `ds.cor` | `y` | – | classes.vector | medium | vector object (doc) `x` is proposed for `x` too; `x` keeps it |
| `ds.cov` | `y` | – | classes.vector | medium | vector object (doc) `x` is proposed for `x` too; `x` keeps it |
| `ds.dataFrame` | `x` | – | classes | medium | object of unknown class  |
| `ds.dataFrame` | `check.rows` | – | roles.checks (open) | high | checks (name) `checks` is proposed for `check.names`, `DataSHIELD.checks` too; `DataSHIELD.checks` keeps it |
| `ds.dataFrame` | `check.names` | – | roles.checks (open) | high | checks (name) `checks` is proposed for `check.rows`, `DataSHIELD.checks` too; `DataSHIELD.checks` keeps it |
| `ds.dataFrameSort` | `sort.key.name` | – | unresolved | low | role unknown  |
| `ds.dataFrameSubset` | `Boolean.operator` | – | unresolved | low | role unknown  |
| `ds.dim` | `x` | – | classes | medium | object of unknown class  |
| `ds.exists` | `x` | – | classes | medium | object of unknown class  |
| `ds.getWGSR` | `index` | – | unresolved | low | role unknown  |
| `ds.glmPredict` | `newdataname` | – | roles.new_object | high | new object (name) `newobj` is proposed for `newobj` too; `newobj` keeps it |
| `ds.heatmapPlot` | `show` | – | roles.method | medium | method (doc lists options) `method` is proposed for `method` too; `method` keeps it |
| `ds.histogram` | `vertical.axis` | – | roles.method | medium | method (doc lists options) `method` is proposed for `method` too; `method` keeps it |
| `ds.look` | `toAggregate` | – | unresolved | low | role unknown  |
| `ds.ls` | `search.filter` | – | unresolved | low | role unknown  |
| `ds.make` | `toAssign` | – | unresolved | low | role unknown  |
| `ds.metadata` | `x` | – | classes | medium | object of unknown class  |
| `ds.mice` | `newobj_mids` | – | roles.new_object | medium | new object (doc) `newobj` is proposed for `newobj_df` too |
| `ds.mice` | `newobj_df` | – | roles.new_object | medium | new object (doc) `newobj` is proposed for `newobj_mids` too |
| `ds.ns` | `knots` | – | unresolved | low | role unknown  |
| `ds.ns` | `Boundary.knots` | – | unresolved | low | role unknown  |
| `ds.ranksSecure` | `output.ranks.df` | – | roles.new_object | medium | new object (doc) `newobj` is proposed for `summary.output.ranks.df` too |
| `ds.ranksSecure` | `summary.output.ranks.df` | – | roles.new_object | medium | new object (doc) `newobj` is proposed for `output.ranks.df` too |
| `ds.ranksSecure` | `ranks.sort.by` | – | roles.method | medium | method (doc lists options) `method` is proposed for `NA.manage` too |
| `ds.ranksSecure` | `NA.manage` | – | roles.method | medium | method (doc lists options) `method` is proposed for `ranks.sort.by` too |
| `ds.rep` | `source.times` | – | unresolved | low | role unknown  |
| `ds.rep` | `source.length.out` | – | unresolved | low | role unknown  |
| `ds.rep` | `source.each` | – | unresolved | low | role unknown  |
| `ds.reShape` | `direction` | – | unresolved | low | role unknown  |
| `ds.rm` | `x.names` | – | unresolved | low | role unknown  |
| `ds.sample` | `x` | – | roles.new_object | medium | new object (doc) `newobj` is proposed for `newobj` too; `newobj` keeps it |
| `ds.setDefaultOpals` | `opal.name` | – | unresolved | low | role unknown  |
| `ds.table` | `useNA` | – | roles.method | medium | method (doc lists options) `method` is proposed for `force.nfilter` too |
| `ds.table` | `force.nfilter` | – | roles.method | medium | method (doc lists options) `method` is proposed for `useNA` too |
| `ds.testObjExists` | `test.obj.name` | – | classes | medium | object of unknown class  |
| `ds.unList` | `x.name` | – | classes | medium | object of unknown class  |
| `ds.vectorCalc` | `calc` | – | unresolved | low | role unknown  |

### Proposed renames

| Function | Current | Proposed | Rule | Confidence | Reason |
|---|---|---|---|---|---|
| `ds.asDataMatrix` | `x.name` | `mat` | classes.matrix | high | matrix object (doc)  |
| `ds.asFactor` | `input.var.name` | `x` | classes.vector | high | vector object (doc)  |
| `ds.asFactor` | `newobj.name` | `newobj` | roles.new_object | high | new object (name)  |
| `ds.asFactorSimple` | `input.var.name` | `x` | classes.vector | high | vector object (doc)  |
| `ds.asFactorSimple` | `newobj.name` | `newobj` | roles.new_object | high | new object (name)  |
| `ds.asList` | `x.name` | `lst` | classes.list | high | list object (doc)  |
| `ds.asMatrix` | `x.name` | `mat` | classes.matrix | high | matrix object (doc)  |
| `ds.auc` | `pred` | `x` | classes.vector | high | vector object (doc)  |
| `ds.Boole` | `V1` | `x` | multiple_inputs | high | vector object (doc)  |
| `ds.Boole` | `V2` | `y` | multiple_inputs | high | vector object (doc)  |
| `ds.Boole` | `na.assign` | `method` | roles.method | medium | method (doc lists options)  |
| `ds.boxPlot` | `x` | `df` | classes.data.frame | high | data.frame object (doc)  |
| `ds.cbind` | `DataSHIELD.checks` | `checks` | roles.checks (open) | high | checks (name)  |
| `ds.changeRefGroup` | `reorderByRef` | `reorder.by.ref` | style (open) | high | logical value (default/doc)  |
| `ds.colnames` | `x` | `df` | classes.data.frame | medium | data.frame object (doc)  |
| `ds.completeCases` | `x1` | `df` | classes.data.frame | medium | data.frame object (doc)  |
| `ds.cov` | `naAction` | `method` | roles.method | medium | method (doc lists options)  |
| `ds.dataFrame` | `row.names` | `df` | classes.data.frame | high | data.frame object (doc)  |
| `ds.dataFrame` | `stringsAsFactors` | `strings.as.factors` | style (open) | high | logical value (default/doc)  |
| `ds.dataFrame` | `completeCases` | `complete.cases` | style (open) | high | logical value (default/doc)  |
| `ds.dataFrame` | `DataSHIELD.checks` | `checks` | roles.checks (open) | high | checks (name)  |
| `ds.dataFrameFill` | `df.name` | `df` | classes.data.frame | high | data.frame object (doc)  |
| `ds.dataFrameSort` | `df.name` | `df` | classes.data.frame | high | data.frame object (doc)  |
| `ds.dataFrameSort` | `sort.method` | `method` | roles.method | medium | method (doc lists options)  |
| `ds.dataFrameSubset` | `df.name` | `df` | classes.data.frame | high | data.frame object (doc)  |
| `ds.dataFrameSubset` | `V1.name` | `x` | multiple_inputs | high | vector object (doc)  |
| `ds.dataFrameSubset` | `V2.name` | `y` | multiple_inputs | high | vector object (doc)  |
| `ds.dataFrameSubset` | `keep.NAs` | `keep.nas` | style (open) | high | logical value (default/doc)  |
| `ds.forestplot` | `mod` | `lst` | classes.list | medium | list object (doc)  |
| `ds.forestplot` | `variable` | `x` | classes.vector | high | vector object (doc)  |
| `ds.gamlss` | `data` | `df` | classes.data.frame | medium | data.frame object (doc)  |
| `ds.gamlss` | `xvar` | `x` | classes.vector | high | vector object (doc)  |
| `ds.getWGSR` | `sex` | `x` | classes.vector | high | vector object (doc)  |
| `ds.getWGSR` | `firstPart` | `first.part` | style (open) | medium | column (doc)  |
| `ds.getWGSR` | `secondPart` | `second.part` | style (open) | medium | column (doc)  |
| `ds.getWGSR` | `standing` | `method` | roles.method | medium | method (doc lists options)  |
| `ds.getWGSR` | `thirdPart` | `third.part` | style (open) | medium | column (doc)  |
| `ds.glm` | `data` | `df` | classes.data.frame | medium | data.frame object (doc)  |
| `ds.glm` | `CI` | `ci` | style | high | numeric value (doc)  |
| `ds.glm` | `viewIter` | `view.iter` | style (open) | high | logical value (default/doc)  |
| `ds.glm` | `viewVarCov` | `view.var.cov` | style (open) | high | logical value (default/doc)  |
| `ds.glm` | `viewCor` | `view.cor` | style (open) | high | logical value (default/doc)  |
| `ds.glmerSLMA` | `dataName` | `df` | classes.data.frame | medium | data.frame object (doc)  |
| `ds.glmerSLMA` | `control_type` | `control.type` | style (open) | medium | value (doc)  |
| `ds.glmerSLMA` | `control_value` | `control.value` | style (open) | medium | numeric value (doc)  |
| `ds.glmerSLMA` | `nAGQ` | `n.agq` | style (open) | high | numeric value (doc)  |
| `ds.glmerSLMA` | `start_theta` | `start.theta` | style (open) | medium | value (doc)  |
| `ds.glmerSLMA` | `start_fixef` | `start.fixef` | style (open) | medium | value (doc)  |
| `ds.glmPredict` | `output.type` | `method` | roles.method | medium | method (doc lists options)  |
| `ds.glmSLMA` | `dataName` | `df` | classes.data.frame | medium | data.frame object (doc)  |
| `ds.glmSummary` | `x.name` | `model` | classes.model | high | model object (doc)  |
| `ds.hetcor` | `data` | `df` | classes.data.frame | medium | data.frame object (doc)  |
| `ds.hetcor` | `ML` | `ml` | style | high | logical value (default/doc)  |
| `ds.hetcor` | `use` | `x` | classes.vector | high | vector object (doc)  |
| `ds.igb_standards` | `var` | `x` | classes.vector | low | vector object (name only)  |
| `ds.lexis` | `data` | `df` | classes.data.frame | high | data.frame object (doc)  |
| `ds.lexis` | `intervalWidth` | `interval.width` | style (open) | medium | value (doc)  |
| `ds.lexis` | `idCol` | `id.col` | style (open) | medium | column (doc)  |
| `ds.lexis` | `entryCol` | `entry.col` | style (open) | medium | column (doc)  |
| `ds.lexis` | `exitCol` | `exit.col` | style (open) | medium | column (doc)  |
| `ds.lexis` | `statusCol` | `status.col` | style (open) | medium | column (doc)  |
| `ds.lexis` | `expandDF` | `newobj` | roles.new_object | medium | new object (doc)  |
| `ds.list` | `x` | `lst` | classes.list | high | list object (doc)  |
| `ds.lmerSLMA` | `dataName` | `df` | classes.data.frame | medium | data.frame object (doc)  |
| `ds.lmerSLMA` | `REML` | `reml` | style | high | logical value (default/doc)  |
| `ds.lmerSLMA` | `control_type` | `control.type` | style (open) | medium | value (doc)  |
| `ds.lmerSLMA` | `control_value` | `control.value` | style (open) | medium | numeric value (doc)  |
| `ds.lmerSLMA` | `optimizer` | `model` | classes.model | high | model object (doc)  |
| `ds.ls` | `search.GlobalEnv` | `search.global.env` | style (open) | high | logical value (default/doc)  |
| `ds.matrix` | `mdata` | `x` | classes.vector | high | vector object (doc)  |
| `ds.matrix` | `from` | `method` | roles.method | medium | method (doc lists options)  |
| `ds.matrixDet` | `M1` | `mat` | classes.matrix | high | matrix object (doc)  |
| `ds.matrixDet.report` | `M1` | `mat` | classes.matrix | high | matrix object (doc)  |
| `ds.matrixDiag` | `x1` | `x` | classes.vector | high | vector object (doc)  |
| `ds.matrixDiag` | `aim` | `method` | roles.method | medium | method (doc lists options)  |
| `ds.matrixDimnames` | `M1` | `mat` | classes.matrix | high | matrix object (doc)  |
| `ds.matrixInvert` | `M1` | `mat` | classes.matrix | high | matrix object (doc)  |
| `ds.matrixMult` | `M1` | `mat1` | multiple_inputs (open) | high | matrix object (doc)  |
| `ds.matrixMult` | `M2` | `mat2` | multiple_inputs (open) | high | matrix object (doc)  |
| `ds.matrixTranspose` | `M1` | `mat` | classes.matrix | high | matrix object (doc)  |
| `ds.mdPattern` | `x` | `df` | classes.data.frame | medium | data.frame object (doc)  |
| `ds.mean` | `save.mean.Nvalid` | `save.mean.nvalid` | style (open) | high | logical value (default/doc)  |
| `ds.meanByClass` | `x` | `df` | classes.data.frame | medium | data.frame object (doc)  |
| `ds.meanSdGp` | `do.checks` | `checks` | roles.checks (open) | high | checks (name)  |
| `ds.merge` | `x.name` | `df1` | multiple_inputs (open) | high | data.frame object (doc)  |
| `ds.merge` | `y.name` | `df2` | multiple_inputs (open) | high | data.frame object (doc)  |
| `ds.merge` | `suffixes` | `method` | roles.method | medium | method (name/default)  |
| `ds.message` | `message.obj.name` | `lst` | classes.list | high | list object (doc)  |
| `ds.mice` | `data` | `df` | classes.data.frame | medium | data.frame object (doc)  |
| `ds.mice` | `predictorMatrix` | `predictor.matrix` | style (open) | medium | numeric value (doc)  |
| `ds.names` | `xname` | `lst` | classes.list | high | list object (doc)  |
| `ds.ranksSecure` | `input.var.name` | `x` | classes.vector | high | vector object (doc)  |
| `ds.ranksSecure` | `shared.seed.value` | `seed` | roles.seed | high | seed (name)  |
| `ds.rbind` | `DataSHIELD.checks` | `checks` | roles.checks (open) | high | checks (name)  |
| `ds.rBinom` | `seed.as.integer` | `seed` | roles.seed | high | seed (name)  |
| `ds.recodeLevels` | `newCategories` | `new.categories` | style (open) | medium | value (doc)  |
| `ds.rep` | `length.out` | `x` | classes.vector | high | vector object (doc)  |
| `ds.rep` | `source.x1` | `method` | roles.method | medium | method (doc lists options)  |
| `ds.replaceNA` | `forNA` | `lst` | classes.list | high | list object (doc)  |
| `ds.reShape` | `data.name` | `df` | classes.data.frame | high | data.frame object (doc)  |
| `ds.rNorm` | `seed.as.integer` | `seed` | roles.seed | high | seed (name)  |
| `ds.rowColCalc` | `x` | `mat` | classes.matrix | medium | matrix object (doc)  |
| `ds.rowColCalc` | `operation` | `method` | roles.method | medium | method (doc lists options)  |
| `ds.rPois` | `seed.as.integer` | `seed` | roles.seed | high | seed (name)  |
| `ds.rUnif` | `seed.as.integer` | `seed` | roles.seed | high | seed (name)  |
| `ds.sample` | `seed.as.integer` | `seed` | roles.seed | high | seed (name)  |
| `ds.seq` | `FROM.value.char` | `from.value.char` | style (open) | high | numeric value (doc)  |
| `ds.seq` | `BY.value.char` | `by.value.char` | style (open) | high | numeric value (doc)  |
| `ds.seq` | `TO.value.char` | `to.value.char` | style (open) | high | numeric value (doc)  |
| `ds.seq` | `LENGTH.OUT.value.char` | `length.out.value.char` | style (open) | high | numeric value (doc)  |
| `ds.seq` | `ALONG.WITH.name` | `x` | classes.vector | high | vector object (doc)  |
| `ds.setSeed` | `seed.as.integer` | `seed` | roles.seed | high | seed (name)  |
| `ds.standardiseDf` | `df.name` | `df` | classes.data.frame | high | data.frame object (doc)  |
| `ds.standardiseDf` | `fix_class` | `fix.class` | style | high | vector object (doc) descriptive name kept: several vector inputs |
| `ds.standardiseDf` | `fix_levels` | `fix.levels` | style | high | vector object (doc) descriptive name kept: several vector inputs |
| `ds.subset` | `x` | `df` | classes.data.frame | medium | data.frame object (doc)  |
| `ds.subset` | `completeCases` | `complete.cases` | style (open) | high | logical value (default/doc)  |
| `ds.subset` | `cols` | `x` | classes.vector | high | vector object (doc)  |
| `ds.subset` | `logicalOperator` | `logical.operator` | style (open) | high | logical value (default/doc)  |
| `ds.subsetByClass` | `x` | `df` | classes.data.frame | high | data.frame object (doc)  |
| `ds.subsetByClass` | `subsets` | `newobj` | roles.new_object | medium | new object (doc)  |
| `ds.subsetByClass` | `variables` | `x` | classes.vector | high | vector object (doc)  |
| `ds.table` | `cvar` | `x` | classes.vector | high | vector object (doc)  |
| `ds.table1D` | `warningMessage` | `warning.message` | style (open) | high | logical value (default/doc)  |
| `ds.table2D` | `warningMessage` | `warning.message` | style (open) | high | logical value (default/doc)  |
| `ds.tapply.assign` | `X.name` | `x` | classes.vector | high | vector object (doc)  |
| `ds.tapply.assign` | `INDEX.names` | `index.names` | style | high | vector object (doc) descriptive name kept: several vector inputs |
| `ds.tapply` | `X.name` | `x` | classes.vector | high | vector object (doc)  |
| `ds.tapply` | `INDEX.names` | `index.names` | style | medium | vector object (doc) descriptive name kept: several vector inputs |
| `ds.unique` | `x.name` | `x` | classes.vector | high | vector object (doc)  |
| `subsetHelper` | `dts` | `datasources` | roles.connection | high | connection (name/doc)  |
| `subsetHelper` | `data` | `df` | classes.data.frame | medium | data.frame object (doc)  |

### Skipped

None.

## dsBase

### Need a decision

| Function | Current | Proposed | Rule | Confidence | Reason |
|---|---|---|---|---|---|
| `asCharacterDS` | `x.name` | – | classes | medium | object of unknown class  |
| `asIntegerDS` | `x.name` | – | classes | medium | object of unknown class  |
| `asLogicalDS` | `x.name` | – | classes | medium | object of unknown class  |
| `asNumericDS` | `x.name` | – | classes | medium | object of unknown class  |
| `changeRefGroupDS` | `ref` | – | unresolved | low | role unknown  |
| `corDS` | `y` | – | classes.vector | medium | vector object (doc) `x` is proposed for `x` too; `x` keeps it |
| `covDS` | `y` | – | classes.vector | medium | vector object (doc) `x` is proposed for `x` too; `x` keeps it |
| `dataFrameSubsetDS1` | `Boolean.operator.n` | – | unresolved | low | role unknown  |
| `dataFrameSubsetDS2` | `Boolean.operator.n` | – | unresolved | low | role unknown  |
| `dmtC2SDS` | `dfdata.mat.transmit` | – | unresolved | low | role unknown  |
| `dmtC2SDS` | `from` | – | unresolved | low | role unknown  |
| `extractQuantilesDS1` | `extract.quantiles` | – | unresolved | low | role unknown  |
| `getWGSRDS` | `index` | – | unresolved | low | role unknown  |
| `glmerSLMADS.assign` | `control_value.transmit` | – | unresolved | low | role unknown  |
| `glmerSLMADS.assign` | `theta` | – | unresolved | low | role unknown  |
| `glmerSLMADS.assign` | `fixef` | – | unresolved | low | role unknown  |
| `glmerSLMADS2` | `control_value.transmit` | – | unresolved | low | role unknown  |
| `glmerSLMADS2` | `theta` | – | unresolved | low | role unknown  |
| `glmerSLMADS2` | `fixef` | – | unresolved | low | role unknown  |
| `lexisDS2` | `intervalWidth` | – | unresolved | low | role unknown  |
| `lmerSLMADS.assign` | `control_value.transmit` | – | unresolved | low | role unknown  |
| `lmerSLMADS2` | `control_value.transmit` | – | unresolved | low | role unknown  |
| `lsDS` | `search.filter` | – | unresolved | low | role unknown  |
| `miceDS` | `newobj_mids` | – | roles.new_object | medium | new object (doc) `newobj` is proposed for `newobj_df` too |
| `miceDS` | `newobj_df` | – | roles.new_object | medium | new object (doc) `newobj` is proposed for `newobj_mids` too |
| `nsDS` | `knots` | – | unresolved | low | role unknown  |
| `nsDS` | `Boundary.knots` | – | unresolved | low | role unknown  |
| `repDS` | `source.times` | – | unresolved | low | role unknown  |
| `repDS` | `source.length.out` | – | unresolved | low | role unknown  |
| `repDS` | `source.each` | – | unresolved | low | role unknown  |
| `tableDS.assign` | `rvar.all.unique.levels.transmit` | – | unresolved | low | role unknown  |
| `tableDS.assign` | `cvar.all.unique.levels.transmit` | – | unresolved | low | role unknown  |
| `tableDS.assign` | `stvar.all.unique.levels.transmit` | – | unresolved | low | role unknown  |
| `tableDS.assign` | `exclude.transmit` | – | unresolved | low | role unknown  |
| `tableDS.assign` | `useNA.transmit` | – | unresolved | low | role unknown  |
| `tableDS` | `rvar.all.unique.levels.transmit` | – | unresolved | low | role unknown  |
| `tableDS` | `cvar.all.unique.levels.transmit` | – | unresolved | low | role unknown  |
| `tableDS` | `stvar.all.unique.levels.transmit` | – | unresolved | low | role unknown  |
| `tableDS` | `exclude.transmit` | – | unresolved | low | role unknown  |
| `tableDS` | `useNA.transmit` | – | unresolved | low | role unknown  |
| `tableDS` | `force.nfilter.transmit` | – | unresolved | low | role unknown  |
| `unListDS` | `x.name` | – | classes | medium | object of unknown class  |

### Proposed renames

| Function | Current | Proposed | Rule | Confidence | Reason |
|---|---|---|---|---|---|
| `asDataMatrixDS` | `x.name` | `mat` | classes.matrix | high | matrix object (doc)  |
| `asFactorDS1` | `input.var.name` | `x` | classes.vector | medium | column (doc) follows client ds.asFactor(input.var.name) |
| `asFactorDS2` | `input.var.name` | `x` | classes.vector | medium | column (doc) follows client ds.asFactor(input.var.name) |
| `asFactorDS2` | `all.unique.levels.transmit` | `x.transmit` | classes.vector | high | vector object (doc)  |
| `asFactorSimpleDS` | `input.var.name` | `x` | classes.vector | medium | column (doc) follows client ds.asFactorSimple(input.var.name) |
| `asListDS` | `x.name` | `lst` | classes.list | high | matrix object (doc) follows client ds.asList(x.name) |
| `asMatrixDS` | `x.name` | `mat` | classes.matrix | high | matrix object (doc)  |
| `aucDS` | `pred` | `x` | classes.vector | high | vector object (doc)  |
| `blackBoxDS` | `input.var.name` | `x` | classes.vector | medium | vector object (from client ds.ranksSecure(input.var.name))  |
| `blackBoxDS` | `shared.seedval` | `seed` | roles.seed | high | seed (name)  |
| `blackBoxDS` | `NA.manage` | `method` | roles.method | medium | method (from client ds.ranksSecure(NA.manage))  |
| `blackBoxRanksDS` | `input.var.name` | `x` | classes.vector | high | vector object (doc)  |
| `blackBoxRanksDS` | `shared.seedval` | `seed` | roles.seed | high | seed (name)  |
| `BooleDS` | `V1.name` | `x` | multiple_inputs | high | vector object (doc)  |
| `BooleDS` | `V2.name` | `y` | multiple_inputs | high | vector object (doc)  |
| `BooleDS` | `Boolean.operator.n` | `boolean.operator.n` | style (open) | high | numeric value (doc)  |
| `BooleDS` | `na.assign.text` | `method` | roles.method | medium | method (doc lists options)  |
| `boxPlotGG_data_TreatmentDS` | `table` | `df` | classes.data.frame | high | data.frame object (doc)  |
| `boxPlotGGDS` | `data_table` | `df` | classes.data.frame | high | data.frame object (doc)  |
| `cbindDS` | `x.names.transmit` | `x.transmit` | classes.vector | high | vector object (doc)  |
| `cDS` | `objs` | `lst` | classes.list | high | list object (doc)  |
| `changeRefGroupDS` | `xvect` | `x` | classes.vector | medium | value (doc) follows client ds.changeRefGroup(x) |
| `changeRefGroupDS` | `reorderByRef` | `reorder.by.ref` | style (open) | high | logical value (default/doc)  |
| `colnamesDS` | `x` | `df` | classes.data.frame | medium | data.frame object (doc)  |
| `completeCasesDS` | `x1.transmit` | `df.transmit` | classes.data.frame | medium | data.frame object (doc)  |
| `covDS` | `use` | `method` | roles.method | medium | method (doc lists options)  |
| `dataFrameDS` | `vectors` | `lst` | classes.list | medium | list object (doc)  |
| `dataFrameDS` | `r.names` | `x` | classes.vector | high | vector object (doc)  |
| `dataFrameDS` | `strAsFactors` | `strings.as.factors` | style (open) | high | logical value (default/doc) follows client ds.dataFrame(stringsAsFactors) |
| `dataFrameDS` | `completeCases` | `complete.cases` | style (open) | high | logical value (default/doc)  |
| `dataFrameFillDS` | `df.name` | `df` | classes.data.frame | high | data.frame object (doc)  |
| `dataFrameFillDS` | `allNames.transmit` | `all.names.transmit` | style | high | vector object (doc) descriptive name kept: several vector inputs |
| `dataFrameSortDS` | `df.name` | `df` | classes.data.frame | high | data.frame object (doc)  |
| `dataFrameSortDS` | `sort.key.name` | `x` | classes.vector | high | vector object (doc)  |
| `dataFrameSortDS` | `sort.method` | `method` | roles.method | medium | method (from client ds.dataFrameSort(sort.method))  |
| `dataFrameSubsetDS1` | `df.name` | `df` | classes.data.frame | high | data.frame object (doc)  |
| `dataFrameSubsetDS1` | `V1.name` | `x` | multiple_inputs | high | vector object (doc)  |
| `dataFrameSubsetDS1` | `V2.name` | `y` | multiple_inputs | high | vector object (doc)  |
| `dataFrameSubsetDS1` | `keep.NAs` | `keep.nas` | style (open) | high | logical value (default/doc)  |
| `dataFrameSubsetDS2` | `df.name` | `df` | classes.data.frame | high | data.frame object (doc)  |
| `dataFrameSubsetDS2` | `V1.name` | `x` | multiple_inputs | high | vector object (doc)  |
| `dataFrameSubsetDS2` | `V2.name` | `y` | multiple_inputs | high | vector object (doc)  |
| `dataFrameSubsetDS2` | `keep.NAs` | `keep.nas` | style (open) | high | logical value (default/doc)  |
| `densityGridDS` | `xvect` | `x` | multiple_inputs | medium | value (doc) follows client ds.contourPlot(x) |
| `densityGridDS` | `yvect` | `y` | multiple_inputs | medium | value (doc) follows client ds.contourPlot(y) |
| `dimDS` | `x` | `df` | classes.data.frame | medium | data.frame object (doc) client callers differ: ds.rowColCalc(x -> mat), ds.subsetByClass(x -> df), ds.summary(x -> x), subsetHelper(data -> df) |
| `dmtC2SDS` | `inout.object.transmit` | `method.transmit` | roles.method | medium | method (doc lists options)  |
| `dmtC2SDS` | `nrows.transmit` | `mat.transmit` | classes.matrix | high | matrix object (doc)  |
| `extractQuantilesDS1` | `extract.summary.output.ranks.df` | `newobj` | roles.new_object | medium | new object (doc)  |
| `extractQuantilesDS2` | `extract.summary.output.ranks.df` | `newobj` | roles.new_object | medium | new object (doc)  |
| `gamlssDS` | `data` | `df` | classes.data.frame | medium | data.frame object (doc)  |
| `gamlssDS` | `xvar` | `x` | classes.vector | high | vector object (doc)  |
| `getWGSRDS` | `sex` | `x` | classes.vector | high | vector object (doc)  |
| `getWGSRDS` | `firstPart` | `first.part` | style (open) | medium | column (doc)  |
| `getWGSRDS` | `secondPart` | `second.part` | style (open) | medium | column (doc)  |
| `getWGSRDS` | `standing` | `method` | roles.method | medium | method (doc lists options)  |
| `getWGSRDS` | `thirdPart` | `third.part` | style (open) | medium | column (doc)  |
| `glmDS1` | `data` | `df` | classes.data.frame | medium | data.frame object (doc)  |
| `glmDS2` | `dataName` | `df` | classes.data.frame | medium | data.frame object (doc)  |
| `glmerSLMADS.assign` | `dataName` | `df` | classes.data.frame | medium | data.frame object (from client ds.glmerSLMA(dataName))  |
| `glmerSLMADS.assign` | `control_type` | `control.type` | style (open) | medium | value (from client ds.glmerSLMA(control_type))  |
| `glmerSLMADS.assign` | `nAGQ` | `n.agq` | style (open) | high | numeric value (doc)  |
| `glmerSLMADS2` | `dataName` | `df` | classes.data.frame | medium | data.frame object (from client ds.glmerSLMA(dataName))  |
| `glmerSLMADS2` | `control_type` | `control.type` | style (open) | medium | value (from client ds.glmerSLMA(control_type))  |
| `glmerSLMADS2` | `nAGQ` | `n.agq` | style (open) | high | numeric value (doc)  |
| `glmPredictDS.ag` | `newdataname.transmit` | `df.transmit` | classes.data.frame | high | data.frame object (doc)  |
| `glmPredictDS.ag` | `output.type` | `method` | roles.method | medium | method (doc lists options)  |
| `glmPredictDS.as` | `newdataname.transmit` | `df.transmit` | classes.data.frame | high | data.frame object (doc)  |
| `glmPredictDS.as` | `output.type` | `method` | roles.method | medium | method (doc lists options)  |
| `glmSLMADS.assign` | `offsetName` | `offset.name` | style | high | vector object (doc) descriptive name kept: several vector inputs |
| `glmSLMADS.assign` | `weightsName` | `weights.name` | style | high | vector object (doc) descriptive name kept: several vector inputs |
| `glmSLMADS.assign` | `dataName` | `df` | classes.data.frame | medium | data.frame object (doc)  |
| `glmSLMADS1` | `data` | `df` | classes.data.frame | medium | data.frame object (doc)  |
| `glmSLMADS2` | `dataName` | `df` | classes.data.frame | medium | data.frame object (doc)  |
| `glmSummaryDS.ag` | `x.transmit` | `model.transmit` | classes.model | high | model object (doc)  |
| `glmSummaryDS.as` | `x.transmit` | `model.transmit` | classes.model | high | model object (doc)  |
| `hetcorDS` | `data` | `df` | classes.data.frame | medium | data.frame object (doc)  |
| `hetcorDS` | `ML` | `ml` | style | high | logical value (default/doc)  |
| `hetcorDS` | `use` | `x` | classes.vector | high | vector object (doc)  |
| `histogramDS1` | `xvect` | `x` | classes.vector | medium | value (doc) follows client ds.histogram(x) |
| `histogramDS2` | `xvect` | `x` | classes.vector | medium | value (doc) follows client ds.histogram(x) |
| `igb_standardsDS` | `var` | `x` | classes.vector | low | vector object (name only)  |
| `isNaDS` | `xvect` | `x` | classes.vector | medium | value (doc) follows client ds.isNA(x) |
| `isValidDS` | `obj` | `x` | classes.vector | medium | value (doc) follows client ds.isValid(x) |
| `lexisDS1` | `exitCol` | `exit.col` | style (open) | high | vector object (doc) follows client ds.lexis(exitCol) |
| `lexisDS2` | `datatext` | `df` | classes.data.frame | high | data.frame object (doc)  |
| `lexisDS2` | `idCol` | `id.col` | style | high | vector object (doc) descriptive name kept: several vector inputs |
| `lexisDS2` | `entryCol` | `entry.col` | style | high | vector object (doc) descriptive name kept: several vector inputs |
| `lexisDS2` | `exitCol` | `exit.col` | style | high | vector object (doc) descriptive name kept: several vector inputs |
| `lexisDS2` | `statusCol` | `status.col` | style | high | vector object (doc) descriptive name kept: several vector inputs |
| `lexisDS2` | `vartext` | `variables` | style | medium | column (doc) follows client ds.lexis(variables) |
| `lmerSLMADS.assign` | `dataName` | `df` | classes.data.frame | medium | data.frame object (from client ds.lmerSLMA(dataName))  |
| `lmerSLMADS.assign` | `REML` | `reml` | style | high | logical value (default/doc)  |
| `lmerSLMADS.assign` | `control_type` | `control.type` | style (open) | medium | value (from client ds.lmerSLMA(control_type))  |
| `lmerSLMADS.assign` | `optimizer` | `model` | classes.model | medium | model object (from client ds.lmerSLMA(optimizer))  |
| `lmerSLMADS2` | `dataName` | `df` | classes.data.frame | medium | data.frame object (from client ds.lmerSLMA(dataName))  |
| `lmerSLMADS2` | `REML` | `reml` | style | high | logical value (default/doc)  |
| `lmerSLMADS2` | `control_type` | `control.type` | style (open) | medium | value (from client ds.lmerSLMA(control_type))  |
| `lmerSLMADS2` | `optimizer` | `model` | classes.model | medium | model object (from client ds.lmerSLMA(optimizer))  |
| `matrixDetDS1` | `M1.name` | `mat` | classes.matrix | high | matrix object (doc)  |
| `matrixDetDS2` | `M1.name` | `mat` | classes.matrix | high | matrix object (doc)  |
| `matrixDiagDS` | `x1.transmit` | `mat.transmit` | classes.matrix | high | matrix object (doc)  |
| `matrixDiagDS` | `aim` | `method` | roles.method | medium | method (from client ds.matrixDiag(aim))  |
| `matrixDiagDS` | `nrows.transmit` | `x.transmit` | classes.vector | high | vector object (doc)  |
| `matrixDimnamesDS` | `M1.name` | `mat` | classes.matrix | high | matrix object (doc)  |
| `matrixDS` | `from` | `method` | roles.method | high | matrix object (doc) follows client ds.matrix(from) |
| `matrixDS` | `ncols.transmit` | `x.transmit` | classes.vector | high | vector object (doc)  |
| `matrixInvertDS` | `M1.name` | `mat` | classes.matrix | high | matrix object (doc)  |
| `matrixMultDS` | `M1.name` | `mat1` | multiple_inputs (open) | high | matrix object (doc)  |
| `matrixMultDS` | `M2.name` | `mat2` | multiple_inputs (open) | high | matrix object (doc)  |
| `matrixTransposeDS` | `M1.name` | `mat` | classes.matrix | high | matrix object (doc)  |
| `mdPatternDS` | `x` | `df` | classes.data.frame | medium | data.frame object (doc)  |
| `meanDS` | `xvect` | `x` | classes.vector | medium | value (doc) follows client ds.mean(x) |
| `meanSdGpDS` | `X` | `x` | classes.vector | high | vector object (doc)  |
| `meanSdGpDS` | `INDEX` | `y` | multiple_inputs | medium | value (doc) follows client ds.meanSdGp(y) |
| `mergeDS` | `x.name` | `df1` | multiple_inputs (open) | high | data.frame object (doc)  |
| `mergeDS` | `y.name` | `df2` | multiple_inputs (open) | high | data.frame object (doc)  |
| `messageDS` | `message.object.name` | `lst` | classes.list | high | list object (doc)  |
| `miceDS` | `data` | `df` | classes.data.frame | medium | data.frame object (doc)  |
| `miceDS` | `predictorMatrix` | `predictor.matrix` | style (open) | medium | numeric value (doc)  |
| `minMaxRandDS` | `input.var.name` | `x` | classes.vector | medium | vector object (from client ds.ranksSecure(input.var.name))  |
| `namesDS` | `xname.transmit` | `lst.transmit` | classes.list | high | list object (doc)  |
| `numNaDS` | `xvect` | `x` | classes.vector | medium | value (doc) follows client ds.numNA(x) |
| `quantileMeanDS` | `xvect` | `x` | classes.vector | medium | value (doc) follows client ds.quantileMean(x) |
| `ranksSecureDS4` | `ranks.sort.by` | `method` | roles.method | medium | method (doc lists options)  |
| `ranksSecureDS5` | `output.ranks.df` | `newobj` | roles.new_object | medium | new object (doc)  |
| `rbindDS` | `x.names.transmit` | `x.transmit` | classes.vector | high | vector object (doc)  |
| `recodeValuesDS` | `var.name.text` | `var.name` | style | high | vector object (doc) follows client ds.recodeValues(var.name) |
| `repDS` | `source.x1` | `method` | roles.method | medium | method (doc lists options)  |
| `replaceNaDS` | `xvect` | `x` | classes.vector | high | vector object (doc)  |
| `reShapeDS` | `data.name` | `df` | classes.data.frame | high | data.frame object (doc)  |
| `reShapeDS` | `direction` | `method` | roles.method | medium | method (doc lists options)  |
| `rmDS` | `x.names.transmit` | `newobj.transmit` | roles.new_object | high | list object (doc) follows client ds.standardiseDf(newobj) |
| `rowColCalcDS` | `dataset` | `mat` | classes.matrix | medium | matrix object (from client ds.rowColCalc(x))  |
| `sampleDS` | `x.transmit` | `newobj.transmit` | roles.new_object | medium | new object (doc)  |
| `seqDS` | `FROM.value.char` | `from.value.char` | style (open) | medium | numeric value (from client ds.seq(FROM.value.char))  |
| `seqDS` | `TO.value.char` | `to.value.char` | style (open) | medium | numeric value (from client ds.seq(TO.value.char))  |
| `seqDS` | `BY.value.char` | `by.value.char` | style (open) | medium | value (doc)  |
| `seqDS` | `LENGTH.OUT.value.char` | `length.out.value.char` | style (open) | high | numeric value (doc)  |
| `seqDS` | `ALONG.WITH.name` | `x` | classes.vector | medium | column (doc) follows client ds.seq(ALONG.WITH.name) |
| `setSeedDS` | `seedtext` | `seed` | roles.seed | high | seed (name)  |
| `getClassAllColsDS` | `df.name` | `df` | classes.data.frame | high | data.frame object (doc)  |
| `fixClassDS` | `df.name` | `df` | classes.data.frame | high | data.frame object (doc)  |
| `fixClassDS` | `target_vars` | `target.vars` | style | high | vector object (doc) descriptive name kept: several vector inputs |
| `fixClassDS` | `target_class` | `target.class` | style | high | vector object (doc) descriptive name kept: several vector inputs |
| `fixColsDS` | `.data` | `df` | classes.data.frame | high | data.frame object (doc)  |
| `fixColsDS` | `cols` | `x` | classes.vector | high | vector object (doc)  |
| `getAllLevelsDS` | `df.name` | `df` | classes.data.frame | high | data.frame object (doc)  |
| `getAllLevelsDS` | `factor_vars` | `x` | classes.vector | high | vector object (doc)  |
| `fixLevelsDS` | `df.name` | `df` | classes.data.frame | high | data.frame object (doc)  |
| `fixLevelsDS` | `vars` | `x` | classes.vector | high | vector object (doc)  |
| `fixLevelsDS` | `levels` | `lst` | classes.list | medium | list object (doc)  |
| `subsetByClassDS` | `data` | `df` | classes.data.frame | medium | data.frame object (doc)  |
| `subsetByClassDS` | `variables` | `x` | classes.vector | high | vector object (doc)  |
| `subsetDS` | `dt` | `df` | classes.data.frame | medium | data.frame object (doc)  |
| `subsetDS` | `complt` | `complete.cases` | style (open) | high | logical value (default/doc) follows client ds.subset(completeCases) |
| `subsetDS` | `rs` | `rows` | style | medium | value (doc) follows client ds.subset(rows) |
| `subsetDS` | `cs` | `x` | classes.vector | high | vector object (doc) follows client ds.subset(cols) |
| `subsetDS` | `lg` | `logical.operator` | style (open) | medium | value (doc) follows client ds.subset(logicalOperator) |
| `subsetDS` | `th` | `threshold` | style | medium | numeric value (doc) follows client ds.subset(threshold) |
| `table1DDS` | `xvect` | `x` | classes.vector | medium | value (doc) follows client ds.summary(x) |
| `table2DDS` | `xvect` | `x` | multiple_inputs | medium | value (doc) follows client ds.table2D(x) |
| `table2DDS` | `yvect` | `y` | multiple_inputs | medium | value (doc) follows client ds.table2D(y) |
| `tapplyDS.assign` | `X.name` | `x` | classes.vector | high | vector object (doc)  |
| `tapplyDS.assign` | `INDEX.names.transmit` | `x.transmit` | classes.vector | high | vector object (doc)  |
| `tapplyDS` | `X.name` | `x` | classes.vector | high | vector object (doc)  |
| `tapplyDS` | `INDEX.names.transmit` | `x.transmit` | classes.vector | high | vector object (doc)  |
| `testObjExistsDS` | `test.obj.name` | `x` | classes.vector | high | vector object (doc)  |
| `uniqueDS` | `x.name.transmit` | `x.transmit` | classes.vector | high | vector object (doc)  |
| `varDS` | `xvect` | `x` | classes.vector | medium | value (doc) follows client ds.var(x) |

### Skipped

None.

## dsBaseClient: other findings (report only)

**Package:**

- Missing in `DESCRIPTION`: `URL`, `BugReports`.

**Client and server:**

- `ds.replaceNA` calls `, vectorDS`, which `dsBase` doesn't declare.
- Declared, but no client function calls it: `scoreVectDS`, `subsetByClassDS`, `vectorDS`, `c`.

**Function files:**

- `ds.mdPattern.R` holds several functions: `ds.mdPattern`, `.pool_md_patterns`.
- `ds.standardiseDf.R` holds several functions: `ds.standardiseDf`, `.check_arguments`, `.stop_if_cols_identical`, `.get_var_classes`, `.identify_class_conflicts`, `prompt_user_class_decision_all_vars`, `prompt_user_class_decision`, `print_all_classes`, `ask_question_wait_response_class`, `ask_question_class`, `.fix_classes`, `.get_unique_cols`, `.add_missing_cols_to_df`, `.get_added_cols`, `.identify_factor_vars`, `.get_factor_levels`, `.identify_level_conflicts`, `ask_question_wait_response_levels`, `.make_levels_message`, `.get_unique_levels`, `.set_factor_levels`, `.print_out_messages`, `.print_var_recode_message`, `.print_class_recode_message`, `.change_choice_to_string`, `.print_levels_recode_message`, `.make_levels_recode_message`, `.handle_warnings`, `.print_class_warning`.

**Roxygen tags:**

- `ds.asFactorSimple`: missing examples.
- `ds.auc`: missing examples.
- `ds.boxPlot`: missing details, author.
- `ds.bp_standards`: missing details, examples.
- `ds.dmtC2S`: missing examples.
- `ds.elspline`: missing examples.
- `ds.forestplot`: missing details, author.
- `ds.gamlss`: missing examples.
- `ds.glmPredict`: missing examples.
- `ds.glmSummary`: missing examples.
- `ds.hetcor`: missing examples.
- `ds.igb_standards`: missing details, examples.
- `ds.kurtosis`: missing examples.
- `ds.listOpals`: missing examples.
- `ds.lspline`: missing examples.
- `ds.mice`: missing examples.
- `ds.ns`: missing examples.
- `ds.qlspline`: missing examples.
- `ds.ranksSecure`: missing examples.
- `ds.sample`: missing examples.
- `ds.setDefaultOpals`: missing examples, param (opal.name).
- `ds.standardiseDf`: missing title, description, details, examples.
- `ds.table`: missing examples.
- `subsetHelper`: missing author.

**Function names not following the pattern:** `ds.Boole`, `ds.bp_standards`, `ds.igb_standards`, `ds.matrixDet.report`, `ds.tapply.assign`, `subsetHelper`

**`datasources` not last:** `ds.cbind`, `ds.dataFrame`, `ds.dataFrameSubset`, `ds.glmerSLMA`, `ds.lmerSLMA`, `ds.rbind`, `ds.recodeValues`, `ds.sample`, `ds.table`, `subsetHelper`

**Test file names:**

- `test-_-vm-test.R`: name does not match the pattern
- `test-arg-ds.Boole.R`: name does not match the pattern
- `test-arg-ds.foobar.R`: `ds.foobar` is no function of the package
- `test-arg-ds.matrixDet.report.R`: name does not match the pattern
- `test-arg-ds.tapply.assign.R`: name does not match the pattern
- `test-datachk-ANTHRO.R`: name does not match the pattern
- `test-datachk-CLUSTER_INT.R`: name does not match the pattern
- `test-datachk-CLUSTER_SLO.R`: name does not match the pattern
- `test-datachk-CNSIM.R`: name does not match the pattern
- `test-datachk-DISCORDANT.R`: name does not match the pattern
- `test-datachk-DNSIM.R`: name does not match the pattern
- `test-datachk-FACTOR_LEVELS.R`: name does not match the pattern
- `test-datachk-SURVIVAL_EXPAND_WITH_MISSING.R`: name does not match the pattern
- `test-datachk-TESTING.R`: name does not match the pattern
- `test-discctrl-ds.Boole.R`: name does not match the pattern
- `test-expt-ds.reshape.R`: `ds.reshape` is no function of the package
- `test-perf-conndisconn.R`: name does not match the pattern
- `test-perf-void.R`: name does not match the pattern
- `test-smk-checkClass-discordant.R`: name does not match the pattern
- `test-smk-checkClass.R`: name does not match the pattern
- `test-smk-ds.Boole.R`: name does not match the pattern
- `test-smk-ds.matrixDet.report.R`: name does not match the pattern
- `test-smk-ds.tapply.assign.R`: name does not match the pattern
- `test-smk-isDefined.R`: name does not match the pattern

## dsBase: other findings (report only)

**Package:**

- Missing in `DESCRIPTION`: `URL`, `BugReports`.

**Server methods:**

- Declared without a function: `scoreVectDS`.

**Function files:**

- `standardiseDfDS.R` holds several functions: `getClassAllColsDS`, `fixClassDS`, `.convertClass`, `fixColsDS`, `getAllLevelsDS`, `.checkLevelsDisclosure`, `fixLevelsDS`.
- `getClassAllColsDS` is in `standardiseDfDS.R`, expected `getClassAllColsDS.R`.
- `fixClassDS` is in `standardiseDfDS.R`, expected `fixClassDS.R`.
- `fixColsDS` is in `standardiseDfDS.R`, expected `fixColsDS.R`.
- `getAllLevelsDS` is in `standardiseDfDS.R`, expected `getAllLevelsDS.R`.
- `fixLevelsDS` is in `standardiseDfDS.R`, expected `fixLevelsDS.R`.

**Roxygen tags:**

- `asFactorDS1`: missing author.
- `asFactorDS2`: missing author.
- `asFactorSimpleDS`: missing author.
- `boxPlotGG_data_Treatment_numericDS`: missing description, details, author.
- `boxPlotGG_data_TreatmentDS`: missing description, details, author.
- `boxPlotGGDS`: missing details, author.
- `bp_standardsDS`: missing details.
- `histogramDS1`: missing details.
- `igb_standardsDS`: missing details.
- `isNaDS`: missing details.
- `lexisDS3`: missing author.
- `numNaDS`: missing details.
- `quantileMeanDS`: missing details.
- `rangeDS`: missing details.
- `recodeLevelsDS`: missing details.
- `getClassAllColsDS`: missing title, description, details, author.
- `fixClassDS`: missing title, description, details, author.
- `fixColsDS`: missing title, description, details, author.
- `getAllLevelsDS`: missing title, description, details, author.
- `fixLevelsDS`: missing title, description, details, author.

**Function names not following the pattern:** `asFactorDS1`, `dataFrameSubsetDS1`, `extractQuantilesDS1`, `extractQuantilesDS2`, `glmDS1`, `glmDS2`, `glmerSLMADS2`, `glmPredictDS.ag`, `glmSLMADS1`, `glmSLMADS2`, `glmSummaryDS.ag`, `histogramDS1`, `histogramDS2`, `kurtosisDS1`, `kurtosisDS2`, `lexisDS1`, `lmerSLMADS2`, `matrixDetDS1`, `ranksSecureDS1`, `ranksSecureDS3`, `skewnessDS1`, `skewnessDS2`, `tableDS2`, `asFactorDS2`, `BooleDS`, `boxPlotGG_data_TreatmentDS`, `boxPlotGG_data_Treatment_numericDS`, `bp_standardsDS`, `dataFrameSubsetDS2`, `glmerSLMADS.assign`, `glmPredictDS.as`, `glmSLMADS.assign`, `glmSummaryDS.as`, `igb_standardsDS`, `lexisDS2`, `lexisDS3`, `lmerSLMADS.assign`, `matrixDetDS2`, `ranksSecureDS2`, `ranksSecureDS4`, `ranksSecureDS5`, `tableDS.assign`, `tapplyDS.assign`

**`datasources` not last:** none

**Test file names:**

- `test-smk-asFactorDS1.R`: name does not match the pattern
- `test-smk-asFactorDS2.R`: name does not match the pattern
- `test-smk-BooleDS.R`: name does not match the pattern
- `test-smk-bp_standardsDS.R`: name does not match the pattern
- `test-smk-dataFrameSubsetDS1.R`: name does not match the pattern
- `test-smk-dataFrameSubsetDS2.R`: name does not match the pattern
- `test-smk-extract.R`: name does not match the pattern
- `test-smk-igb_standardsDS.R`: name does not match the pattern
- `test-smk-kurtosisDS1.R`: name does not match the pattern
- `test-smk-kurtosisDS2.R`: name does not match the pattern
- `test-smk-skewnessDS1.R`: name does not match the pattern
- `test-smk-skewnessDS2.R`: name does not match the pattern
- `test-smk-tapplyDS.assign.R`: name does not match the pattern

