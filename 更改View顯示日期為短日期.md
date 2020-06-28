<h2>刪除原本產生的代碼</h2>
<code> @Html.DisplayFor(modelItem => item.fDate)</code>
 <h2>輸入新的代碼</h2>
 <code>@DateTime.Parse(item.fDate.ToString()).ToShortDateString()</code>
