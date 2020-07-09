在@using(Html.BeginForm())需改成如下<br/>
@using (Html.BeginForm("Action","Controller",FormMethod.Post,new { enctype="multipart/form-data"}))
