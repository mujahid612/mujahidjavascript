# web_bazar
web jual beli bazar rpl 1
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    
    <title> 10 RPL 1</title>
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
        text-align: left;
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

      select{
        font-size: 20px;
      }

      p{
        font-size: 20px;
      }

      
    </style>
</head>
<body>
<form action="halamanutama.php" method="post">
    <div class ="background">
    <h2 style = "color:purple;">LIAT MENU DAN ATUR PESANAN ANDA</h2>
    <P style="font-size:50px;">===================</P>
    <P style="font-size:50px;">        PESAN      </P>
    <P style="font-size:50px;">===================</P>
    <P>BROWNIS : </P>
    <select name="JUMLAHB">
      <?php
        for ($mgj=0; $mgj < 10; $mgj++) { 
          echo "<option value=$mgj>$mgj</option>";
        }
       
      ?>

      </select><br>
      
      <P style = color:ligthyellow;><img border ="4" src = "brownis.png" alt = "jastip gacoan"  width ="100px" height = "120px"></P>;

      <P>HARGA</P>
      <P>Rp.3,000</P>
      
      
      <P style="font-size:50px;">===================</P>
    <P>CUPCAKE : </P>
    <select name="JUMLAHC">
    <?php
        for ($mhj=0; $mhj < 10; $mhj++) { 
          echo "<option value=$mhj>$mhj</option>";
        }
      ?>

      </select><br>
      
      <P style = color:ligthyellow;><img border ="4" src = "cupcake.png" alt = "jastip gacoan"  width ="100px" height = "120px"></P>;

      <P>HARGA</P>
      <P>Rp.5,000</P>
      
    <P style="font-size:50px;">===================</P>
    <P >PUDING : </P>
    <select name="JUMLAHP">
    <?php
        for ($msj=0; $msj < 10; $msj++) { 
          echo "<option value=$msj>$msj</option>";
        }
      ?>
      
      </select><br>
  
      <P style = color:ligthyellow;><img border ="4" src = "puding.png" alt = "jastip gacoan"  width ="100px" height = "120px"></P>;

      <P>HARGA</P>
      <P>Rp.2,500</P>
      
    <P style="font-size:50px;">===================</P>
    
    <P>BASO BAKAR : </P>
    <select name="JUMLAHBA">
    <?php
        for ($sj=0; $sj < 10; $sj++) { 
          echo "<option value=$sj>$sj</option>";
        }
      ?>
        
      </select><br>

      <P style = color:ligthyellow;><img border ="4" src = "basobakar.png" alt = "jastip gacoan"  width ="100px" height = "120px"></P>;

      <P>HARGA</P>
      <P>Rp.5,000</P>
    <P style="font-size:50px;">===================</P>
    <P>CORNDOG : </P>
    <select name="JUMLAHCO">
    <?php
        for ($urj=0; $urj < 10; $urj++) { 
          echo "<option value=$urj>$urj</option>";
        }
      ?>
        
      </select><br>
      <P>HARGA</P>
      <P>Rp.5,000</P>
    <P style="font-size:50px;">===================</P>
    <P>TAKOYAKI : </P>
    <select name="JUMLAHTA">
    <?php
        for ($ukj=0; $ukj < 10; $ukj++) { 
          echo "<option value=$ukj>$ukj</option>";
        }
      ?>
      </select><br>

      <P style = color:ligthyellow;><img border ="4" src = "takoyaki.png" alt = "jastip gacoan"  width ="100px" height = "120px"></P>;

      <P>HARGA</P>
      <P>Rp.5,000</P>
    
      <P style="font-size:50px;">===================</P>
    <P>MOJITO : </P>
    <select name="JUMLAHM">
    <?php
        for ($ukm=0; $ukm < 10; $ukm++) { 
          echo "<option value=$ukm>$ukm</option>";
        }
      ?>
      </select><br>
      <P style = color:ligthyellow;><img border ="4" src = "mojito.png" alt = "jastip gacoan"  width ="100px" height = "120px"></P>;

      <P>HARGA</P>
      <P>Rp.5,000</P>

    <P style="font-size:50px;">===================</P>
    <P style="font-size:50px;">      ALAMAT       </P>
    
    <label for="antarke">ANTAR KE RUANGAN:</label>
    <input type="text" name="antarke" id="antarke"><br>
    <P>*kalo mau nunguin di sini ketik "-"</P>
    
    
    <P style="font-size:50px;">===================</P>
    <P style="font-size:50px;">        PEMBELI    </P>
    <label for="pemebeli">NAMA PEMBELI:</label>
    <input type="text" name="pembeli" id="pembeli"><br>
    <label for="kelas">KELAS:</label>
    <input type="text" name="kelas" id="kelas"><br>
    

    
    <P style="font-size:50px;">===================</P>

        <input type="submit" name="pesanan1" value="PESAN"><br>

</form>
</body>
</html>
