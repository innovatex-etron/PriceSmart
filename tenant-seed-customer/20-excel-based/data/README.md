 # tenant-seed-bayer

       Data
            111-referencedata-<TypeName>

                This will be excels for reference data.

                It can contain excel file for all reference data or if project is managing reference data some other way this can have important reference file like, context list, locale list if any.
                We should use the number prefix to ensure that loading of reference entities are in the better order. With this approach, We will have more control while loading the reference data for dependent reference entities.

                Ex: 111-refeencedata-locales, 112-refeencedata-sizetype, 113-refeencedata-sizecode # customer-seed-tenant-base
