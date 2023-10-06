<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>

    <style>
        body {
        background-color : skyblue;
        font-family: Arial, sans-serif;
        text-align: center;
        margin-top: 200px;
         background-image:url('<?php echo $url ?>');
        }

        table {
        
          border:1px solid rgb(0, 0, 0);
           margin: 20px auto;
        }
        th
        {
            border:1px solid rgb(36, 152, 187);
            border-collapse: collapse;
            background-color: rgb(104, 90, 233);
            
        }
        td
        {
            border:1px solid rgb(36, 152, 187);
            border-collapse: collapse;
            background-color: rgb(62, 158, 248);
        }

        input[type=submit] {
          font-size: 45px;
          padding: 10px 20px;
          margin: 10px;
          border-radius: 10px;
          border: none;
          background-color: rgb(60, 0, 255);
          color: white;
          cursor: pointer;
        }
        
        input[type=submit]:hover {
          background-color: skyblue;
        }
        
    </style>
</head>
<body>
    <table>
        <tr>
            <Th  class ="ketengah" colspan="9">DATA GURU</Th>
        </tr>
        <tr>
            <th>No</th>
            <th>Nis</th>
            <th>Nama</th>
            <th>Tanggal lahir</th>
            <th>Kelas</th>
            <th>Alamat</th>
            <th>Jenis kelamin</th>
            <th>Agama</th>
            <th>Hobby</th>
            
        </tr>
        <tr>
            <td>25</td>
            <td>134985</td>
            <td>Mujahid Saifurahman</td>
            <td>Rahasia Tuhan</td>
            <td>XI RPL 4</td>
            <td>Cisaranten Kulon</td>
            <td>Waria</td>
            <td>Hindu</td>
            <td>Gamers</td>
        </tr>

        <tr>
            <td>26</td>
            <td>121212</td>
            <td>Nabilah Ardelia Milan</td>
            <td>15 Desember 2006</td>>
            <td>XI RPL 1</td>
            <td>Ujung Berung</td>
            <td>Perempuan</td>
            <td>Islam</td>
            <td>Badminton</td>
        </tr>
        
        <tr>
            <td>30</td>
            <td>132689</td>
            <td>Nugraha Wijaya Saputra</td>
            <td>Rahasia Bidan</td>
            <td>XI RPL 3</td>
            <td>Zibiru</td>
            <td>Transgender</td>
            <td>Budha</td>
            <td>Desain Grafis</td>
        </tr>

    </table>
    <form action="tugas4_nugraha,mujahid,nabilah.html" method="post">
        
    
        <input type="submit" name="dataguru" value="KEMBALI"><br>
        
    </form>
    <br>
   
    
</body>
</html>
