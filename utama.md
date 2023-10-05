<!DOCTYPE html>
<html>
<head>
    
    
    <title>10 RPL 1</title>
    <h1> WARUNG RPL </h1>
    <style>
      <?php

      $url ='background.png';

      ?>
      body {
      background-color : black;
      font-family: Arial, sans-serif;
      text-align: center;
       background-image:url('<?php echo $url ?>');
      }

      h1 {
        margin-top: 80px;
        color: white;
        font-size: 100px;
        font-family: Arial, sans-serif;
      }
      
      form {
        margin-top: 50px;
      }
      .background{
        max-width: 550px;
        width: 100%;
        background: lightyellow;
        margin: 20px auto;
        padding: 30px;
      }

      .background2{
        max-width: 550px;
        width: 100%;
        background: purple;
        margin: 20px auto;
        padding: 30px;
      }
      
      input[type=text] {
        font-size: 24px;
        padding: 10px;
        margin: 10px;
        border-radius: 10px;
        border: none;
        box-shadow: 0 0 5px gray;
        text-align: right;
        width: 300px;
      }
      
      input[type=submit] {
        font-size: 60px;
        padding: 10px 20px;
        margin: 10px;
        border-radius: 10px;
        border: none;
        background-color: purple;
        color: white;
        cursor: pointer;
      }
      
      input[type=submit]:hover {
        background-color: blue;
      }
      
      .result {
        font-size: 36px;
        font-weight: bold;
        margin-top: 50px;
      }

      
    </style>


</head>
<body>
    
  
  <form action="halamanpesan.php" method="post">
        
    
    <input type="submit" name="halamanpesan" value="PESAN"><br>

   </form>
      <P style = color:ligthyellow;><img border ="4" src = "menu.png" alt = "jastip gacoan"  width ="600px" height = "1200px"></P>;
   <div class="background">
      


       <P style="font-size:50px;">===================</P>
       <P style="font-size:45px;">PESANAN :</P>

 
    <?php

    if (isset($_POST['pesanan1'])) {
        $brownis = $_POST['JUMLAHB'] ;
        $cupcake = $_POST['JUMLAHC'];
        $puding= $_POST['JUMLAHP'];
        $basobakar = $_POST['JUMLAHBA'];
        $corndog = $_POST['JUMLAHCO'];
        $takoyaki = $_POST['JUMLAHTA'];
        $mojito = $_POST['JUMLAHM'];
             
        $antarke = $_POST['antarke'];

        $pembeli = $_POST['pembeli'];
        $kelas = $_POST['kelas'];
        

        

        $totalharga = (($brownis * 3000) + ($cupcake * 5000) + ($puding * 2500) + ($basobakar * 5000) + ($corndog * 5000) + ($takoyaki * 5000) + ($mojito * 5000));
        
    
        
        echo "<font size='7pt'>$pembeli ($kelas)</font> <br> ";
        echo "<font size='10pt'> ==================</font> <br> ";

        echo "<font size='5pt'>BROWNIS: $brownis </font> <br> ";
        echo "<font size='5pt'>PUDING: $puding </font> <br> ";
        echo "<font size='5pt'>CUPCAKE: $cupcake </font> <br>";
        echo "<font size='5pt'>BASOBAKAR: $basobakar  </font> <br>";
        echo "<font size='5pt'>CORNDOG: $corndog </font> <br>";
        echo "<font size='5pt'>TAKOYAKI: $takoyaki </font> <br> ";
        echo "<font size='5pt'>MOJITO: $mojito </font> <br> ";
        echo "<font size='10pt'> ==================</font> <br> ";

        echo "<br> ";
        echo "<font size='5pt'> ANTAR KE RUANG: $antarke </font> <br> ";
        echo "<br> ";

        echo "<font size='5pt'>TOTAL HARGA : $totalharga </font> <br>";
        echo "BERIKAN UANG KE KASIR<br> ";
        echo "<font size='10pt'> ==================</font> <br> ";
  
    }
    ?>
    </div>
    
  
</body>
</html>
