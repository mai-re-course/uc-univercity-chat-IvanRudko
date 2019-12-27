# uc-univercity-chat-IvanRudko
uc-univercity-chat-IvanRudko created by GitHub Classroom

***
1-st option is replenished mode before planning
***
If ( StockingPointPeriod.ReplenishedInventoryLevel() - StockingPointPeriod.InventoryMaxQuantity() ) > MaterialPlanning.InventoryTargetThreshold() ) and element.InventoryMaxQuantity() <> 0 - above max condition (we don’t take zero InventoryMaxQuantity into account, because when we don’t have information about inventory max quantity there are no violations) => StockingPointPeriod node will have red or dark red color, depends on HasActiveInventoryMax = true/false
If StockingPointPeriod.ReplanishedInventoryLevel() < 0 => StockingPointPeriod node will have red or dark red color, depends on HasActiveInventoryMax = true/false
2-nd option is replenished mode after planning
***
If ( StockingPointPeriod.PlannedInventoryLevel() - StockingPointPeriod.InventoryMaxQuantity() ) > CapacityPlanning.InventoryTargetThreshold() ) and element.InventoryMaxQuantity() <> 0 - above max condition (we don’t take zero InventoryMaxQuantity into account, because when we don’t have information about inventory max quantity there are no violations) => StockingPointPeriod node will have red or dark red color, depends on HasActiveInventoryMax = true/false
***
If StockingPointPeriod.PlannedInventoryLevel() < 0 => StockingPointPeriod node will have red or dark red color, depends on HasActiveInventoryMax = true/false
Test cases
***
Change in matrix InventoryTargetSettingsSP Enabled value for stocking point that has any violations
( belowmin or abovemax )
Check if color of the GC node was changed according to color legend
***
Change StockingPointPeriod.PlannedInventoryLevel() value for after planning mode to get into range belowmin or abovemax
Check if GC StockingPointPeriod node colors according to color legend
***
Change StockingPointPeriod.ReplenishedInventoryLevel() value for before planning mode to get into range belowmin or abovemax
Check if GC StockingPointPeriod node colors according to color legend
