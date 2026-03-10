# tenant-seed-bayer

    20-excel-based
        Models
            010-base-model-thing.xlsx
                Excel of base model for thing domain.
            020-base-model-digital-asset.xlsx
                Excel of base model for digital asset domain.
            030-base-model-party.xlsx
                Excel of base model for party domain.
            040-base-model-location.xlsx
                Excel of base model for location domain.
            050-base-model-reference-data.xlsx
                Excel of base model for reference data.
            060-authorization-model.xlsx
                Excel of auth models
            070-taxonomy-model.xlsx
                Excel of taxonomy model
            080-governance-model.xlsm
                Excel of governance model
            100-instance-model.xlsx
                Excel for context model
            110-workflow-model.xlsx
                Excel for workflow model
        Data
            111-referencedata-<TypeName>

                This will be excels for reference data.

                It can contain excel file for all reference data or if project is managing reference data some other way this can have important reference file like, context list, locale list if any.
                We should use the number prefix to ensure that loading of reference entities are in the better order. With this approach, We will have more control while loading the reference data for dependent reference entities.

                Ex: 111-refeencedata-locales, 112-refeencedata-sizetype, 113-refeencedata-sizecode 

        Important Note

        Important Notes :
            It is mandatory to keep same file name of the file followed by some custom post fix.
            you are allowed to create more than one file but making sure file name begins with this name and followed by some meaningful post-fix. This is the case when you might have created governance excel seperate for each entity type or country or any other logical project division. And this can be for any model excel.
                Country post-fix
                Region post-fix
                Entitytype name post-fix
            If you number of files for any model has increased significantly you can create the folder with that model name and keep excels under that folder.
                For example you have one auth model for each countries, you can create folder with name "060-authorization-model" and keep all auth model files under that folder. You need to still follow the excel file naming convensions.
                No ambiguity is allowed between the file unless there is specific reason
            For example GIT should not have file with post-fix like "_backup" , "_old" or "_<date>"
                File available on the GIT needs to be approved version of the model which can be imported to environment