# codiant-gii-model

Model generator--
�	It is used to generates separate model classes to customize ,base and query models classes to regenerate.
�	Use different templates for model generation.

Use custom generators, model templates (Define it in main-local.php)--

$config['modules']['gii'] = [
        'class' => 'yii\gii\Module', 
         'generators' => [
            'model' => [
               	 'class' => 'frontend\codiant\model\Generator',
		'templates' => [   //setting for out templates
                   			 'model' => '@frontend/codiant/model/default', 
               	            	             ]
                                ]
                           ],
                     ];

namespaces--

	1.customize class-
			namespace common\models;
	2.Base class-
			namespace common\models\base;
	3.Query class-
			namespace common\models\query;
