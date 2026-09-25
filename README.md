<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>KHALIF-BUS</title>

<style>
*{box-sizing:border-box}
body{
  margin:0;
  font-family:Arial,sans-serif;
  background:#f4f6f8;
  color:#17202a;
}
header{
  background:#111827;
  color:white;
  padding:20px;
  text-align:center;
}
header h1{margin:0;font-size:28px}
header p{margin:7px 0 0;color:#cbd5e1}

.container{
  max-width:900px;
  margin:auto;
  padding:20px;
}

.card{
  background:white;
  padding:20px;
  margin-bottom:20px;
  border-radius:14px;
  box-shadow:0 3px 12px rgba(0,0,0,.08);
}

h2{margin-top:0}

label{
  display:block;
  margin-top:14px;
  font-weight:bold;
}

input,select{
  width:100%;
  padding:13px;
  margin-top:6px;
  border:1px solid #d1d5db;
  border-radius:8px;
  font-size:16px;
}

button{
  border:0;
  border-radius:9px;
  padding:13px 18px;
  margin-top:16px;
  font-size:16px;
  font-weight:bold;
  cursor:pointer;
  background:#111827;
  color:white;
}

button:hover{opacity:.9}

.seats{
  display:grid;
  grid-template-columns:repeat(4,1fr);
  gap:10px;
  margin-top:15px;
}

.seat{
  padding:12px 5px;
  background:#e5e7eb;
  color:#111827;
  text-align:center;
  border-radius:8px;
  cursor:pointer;
  font-weight:bold;
}

.seat.selected{
  background:#16a34a;
  color:white;
}

.seat.booked{
  background:#dc2626;
  color:white;
  cursor:not-allowed;
}

.summary{
  background:#f1f5f9;
  padding:15px;
  border-radius:10px;
  margin-top:15px;
}

.stats{
  display:grid;
  grid-template-columns:repeat(3,1fr);
  gap:12px;
}

.stat{
  background:#111827;
  color:white;
  padding:18px;
  border-radius:12px;
  text-align:center;
}

.stat strong{
  display:block;
  font-size:24px;
  margin-top:5px;
}

.booking{
  border:1px solid #e5e7eb;
  padding:15px;
  border-radius:10px;
  margin-top:10px;
}

.success{
  background:#dcfce7;
  color:#166534;
  padding:15px;
  border-radius:10px;
  margin-top:15px;
  display:none;
}

@media(max-width:600px){
  .stats{grid-template-columns:1fr}
  .seats{grid-template-columns:repeat(4,1fr)}
}
</style>
</head>
