     Ext.define('myWfs', {
                extend: 'Ext.data.Model',
                fields: ['Name', 'Title']
            });
              
      
            var wfs_capab_store = Ext.create('Ext.data.Store', {
                model: 'myWfs',
                proxy: {
                    type: 'ajax',
                    url : 'geoserver-getCapabilities.xml',
                    reader: {
                        type: 'xml',
                        record: 'FeatureType',
                        rootProperty: 'FeatureTypeList'
                    }
                }
            });
