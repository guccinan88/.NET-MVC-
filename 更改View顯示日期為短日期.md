刪除原本產生的代碼
 @Html.DisplayFor(modelItem => item.fDate)
 輸入新的代碼
 @DateTime.Parse(item.fDate.ToString()).ToShortDateString()
