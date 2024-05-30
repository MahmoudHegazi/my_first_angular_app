# my first angular 5/30/2024


![image](https://github.com/MahmoudHegazi/my_first_angular_app/assets/55125302/111a1b3e-14cf-4b39-81a5-d901bfb8ed8a)


![image](https://github.com/MahmoudHegazi/my_first_angular_app/assets/55125302/101ac306-5b9f-4b3f-b8a0-d063e1311e51)

# what if i asked to create framework like angular what would be like
also this displays how i see angular and how it works plain, note the script is shortest and not valid js it js plain of all steps to do action fast shortelized
```javascript
    pk-model="test"
    function updateView() {
    // update pk-if directives type to update View
    const viewModels = {
    
    };
    const models = ['test']
    
    $("[pk-if]").hide();
    pk-if="test"
    const allPkIfs = Array.from($("[pk-if]"));
    allPkIfs.forEach((elm)=>{
      models.forEach((model)=>{
        if ($(elm).attr('pk-if') == model){
            if (!Array.isArray(viewModels[model])){
               viewModels[model] = [];
            }
            viewModels[model].push({elm, elmParent: $(elm).parent()});
        }
      });
      
    });
    $("[pk-if]").remove(); // here not angular full reupdate
      viewModels[model].forEach((elmWillAddedToView)=>elmWillAddedToView.parent.append(elmWillAddedToView.elm));
    }

    //this simple full update framework angular mentioned partialy update based on model changed not delete all model elms with if in pk-if example
    updateView();
    

```
