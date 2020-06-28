<h2>刪除原本產生的代碼</h2>
 @Html.DisplayFor(modelItem => item.fDate)
 <h2>輸入新的代碼</h2>
 @DateTime.Parse(item.fDate.ToString()).ToShortDateString()
