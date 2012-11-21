


# Dartling Skeleton

Categories: [Dartling] (https://github.com/dzenanr/dartling), new project, code generation.

Description: Dartling Skeleton is a [Dart Editor] 
(http://www.dartlang.org/docs/editor/getting-started/) project template for a new Dartling project.

## Dartling Code Generation Guide

### Your Dartling Project

#### Design a model in [Magic Boxes] (https://github.com/dzenanr/magic_boxes)

* do not use special characters in any names
* do not use - (minus) or space in any names
* do not use plural for box (concept) names
* start a box name with a capital letter
* do not use composite box names (no: CarBrand; yes: Brand);
   if you must use a composite box name, then use [CamelCase]
   (http://en.wikipedia.org/wiki/CamelCase)
* some boxes must be entry
* do not use oid, id, code or concept to name an item
* start an item name with a small letter
* do not repeat the concept name within the attribute name
* item names may be composite 
* for composite item names use camelCase (first letter lower)
* all items must be typed
* all lines must have parent and child names (neighbor names)
* start a neighbor name with a lower letter
* neighbor names may be composite 
* for composite neighbor names use camelCase (first letter lower)
* click on From JSON to obtain the JSON text for the model
* click on Pretty JSON to obtain the formatted JSON text 

#### Copy the dartling_skeleton project

* do not use special characters in any names
* do not use - (minus) or space in any names
* do not use plural for domain and model names
* start a domain name or a model name with a capital letter
* do not use composite names for domains and models 
   (no: DartlingDomain; yes: Dartling);
   if you must use a composite name, then use CamelCase   
* when domain, model or concept names are used in folder and file names, they must be all in lower letters
* when domain, model or concept names are used in folder and file names, if they are used together, they must be separated by _ (underscore): domain_model
* when domain, model or concept names are used in folder and file names, if they are composite, their components must be separated by _ : my_domain
* copy the dartling_skeleton folder and rename it to your domain_name_model_name
* delete the copied .git folder in the new project
* Open Folder... in Dart Editor of the new project
* select the root folder and choose in the pop-up menu Don’t Analyze
* in the web/img and web/dartling/skeleton/img folders replace the png file with your model’s png file
* rename folders, files in the lib, test and web folders that have dartling and skeleton names
* rename dartling with your domain_name
* rename skeleton with your model_name
* do not rename the model.dart file in lib/dartling/skeleton/json
* do not rename the models.dart file in lib/gen/dartling
* update library and part in the library files, lib/dartling_skeleton.dart and lib/dartling_skeleton_app.dart, to reflect your domain and model names
* do not rename import "package:dartling/dartling.dart"; and import "package:dartling/dartling_app.dart";
* in lib/dartling/skeleton/json/data.dart, rename the dartlingSkeletonDataJson var name:
      change dartling to yourDomainName
      change Skeleton to YourModelName
* in lib/dartling/skeleton/json/model.dart, rename the dartlingSkeletonModelJson var name:
      change dartling to yourDomainName;
      change Skeleton to YourModelName;
      do not change model or Model
* in test/dartling/skeleton/dartling_skeleton_gen.dart, rename import "package:dartling_skeleton/dartling_skeleton.dart":
    rename dartling to yourDomainName;
    change "Dartling" to "YourDomainName";
    rename Skeleton to YourModelName;
    change "Skeleton" to "YourModelName"
* copy the pretty format of the JSON text of the model to lib/dartling/skeleton/json/model.dart between var and '''
* Dart Editor must know where you have installed git; on Windows add something like C:\Program Files (x86)\Git\bin; to the Path system variable (http://www.itechtalk.com/thread3595.html)
* move the pub/pubspec.yaml file (file only) to the root folder of your project
* delete the empty pub folder
* rename name in pubspec.yaml
* Close and then open the project folder with the pub
* select the root folder and choose in the pop-up menu Analyze
* Run dartling_skeleton_gen.dart in the test folder to generate code
* copy the generated code into indicated files (including dartling_skeleton_gen) and save; if there is no indicated file, File/New File in its folder
* if red color, close and open the project folder to potentially get rid of some red color
* if there are still errors, check your model in Magic Boxes (read again the recommendations)
* change the model and put the code with red color in comments 
* update at least src of the script tag in dartling_skeleton_web.html file
* init model with some data in lib/dartling/skeleton/init.dart
* Run dartling_skeleton_gen.dart to init
* Run in Dartium web/dartling/skeleton/dartling_skeleton_web.html to see the model alive
* add some tests in the test folder, in dartling_skeleton_test.dart file
* Run dartling_skeleton_test.dart file to test




