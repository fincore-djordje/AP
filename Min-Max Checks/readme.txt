########################################################################################
Content:
    - T1 - STG, ERR, CND
        * 1-Metadata
            + min-max-checks_no_WF.json (for 3 partitions)
            + T1-EntityCleaningWorkflowDaily TemplateV2.JSON
        * 2-Data
            + min-max-checks-dataset.csv
        * 3-DataVisualization
            + T1_Min_Max_Checks_Notebook.json
            + 2021-03-03 17_49_50-Zeppelin.png
    - T2 - STG, ERR, CND, DUP, CMP, RCP
        * 1-Metadata
            + min-max-checks_no_WF.json (for 6 partitions)
            + T1-EntityCleaningWorkflowDaily TemplateV2.JSON
        * 2-Data
            + min-max-checks-dataset_T2.csv
        * 3-DataVisualization
            + T2_Min_Max_Checks_Notebook.json
            + 2021-03-03 18_06_23-Zeppelin.png

    - readme.txt

################################################################################################
#   T1 - STG, ERR, CND                  #
#########################################

T1 - STG, ERR, CND > 1-Metadata > min-max-checks_no_WF.json - file contains just
details about schema, entity and columns. Without workflow, tables, outputs, filters...
Just Schema and Entity, including min and max properties.

------------------------------------------------------------------------------------------------
T1 - STG, ERR, CND > 1-Metadata > T1-EntityCleaningWorkflowDaily TemplateV2.JSON -
necessary template for this metadata, with 3 partitions, STG, ERR, CND.

------------------------------------------------------------------------------------------------
T1 - STG, ERR, CND > 2-Data > min-max-checks-dataset.csv - dataset contains 4 columns:
    1. MinMax           (column)
    2. Min              (column)
    3. Max              (column)
    4. ExpectedOutcome  (column)

------------------------------------------------------------------------------------------------
T1 - STG, ERR, CND > 3-DataVisualization > T1_Min_Max_Checks_Notebook.json - Zeppelin notebook
ready for import.

Expected values:
    1. STG: 54
    2. ERR: 16
    3. CND: 38

    *NOTE: SUM(csv rows) = 54

------------------------------------------------------------------------------------------------
T1 - STG, ERR, CND > 3-DataVisualization > 2021-03-03 17_49_50-Zeppelin.png - screenshot of
data visualization in Zeppelin.

################################################################################################
#   T2 - STG, ERR, CND, DUP, CMP, RCP   #
#########################################

T2 - STG, ERR, CND, DUP, CMP, RCP > 1-Metadata > min-max-checks_no_WF.json - file contains
just details about schema, entity and columns. Without workflow, tables, outputs, filters...
Just Schema and Entity, including min, max, identifier, version, and timestamp, properties.

------------------------------------------------------------------------------------------------
T2 - STG, ERR, CND, DUP, CMP, RCP > T2-ReferenceData (with Duplication checks) Template.JSON -
necessary template for this metadata, with 3 partitions, STG, ERR, CND.

------------------------------------------------------------------------------------------------
T2 - STG, ERR, CND, DUP, CMP, RCP > 2-Data > min-max-checks-dataset_T2.csv - dataset contains
7 columns:
    1. MinMax           (column)
    2. Min              (column)
    3. Max              (column)
    4. ExpectedOutcome  (column)
    5. Index            (column)
    6. Version          (column)
    7. Unique_value     (column)

------------------------------------------------------------------------------------------------
T2 - STG, ERR, CND, DUP, CMP, RCP > 3-DataVisualization > T2_Min_Max_Checks_Notebook.json -
Zeppelin notebook ready for import.

Expected values:
    1. STG: 56
    2. ERR: 39
    3. CND: 15
    4. DUP: 4
    5. CMP: 15
    6. RCP: 56
    
    *NOTE: SUM(csv rows) = 56
------------------------------------------------------------------------------------------------
T2 - STG, ERR, CND, DUP, CMP, RCP > 3-DataVisualization > 2021-03-03 18_06_23-Zeppelin.png -
screenshot of data visualization in Zeppelin.

################################################################################################
#    Updated: 03/03/2021    #
#############################