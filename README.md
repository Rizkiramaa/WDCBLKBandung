<!DOCTYPE html>
<html lang="id">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>Inventaris</title>
  <link rel="stylesheet" href="css/styles.css" />
  <style>
    body {
      font-family: Arial, sans-serif;
      background-color: #d0e7f9; /* biru muda */
      display: flex;
      flex-direction: column;
      align-items: center;
      padding-top: 40px;
    }

    .logo {
      width: 100px;
      margin-bottom: 10px;
    }

    h1 {
       text-align: center;
  margin-bottom: 30px;
  color: black;
  background: linear-gradient(60deg,#192e47 ,#167d38 );
  -webkit-background-clip: text;
  -webkit-text-fill-color: transparent;
  background-clip: text;
    }

    form#loanForm {
      display: flex;
      flex-direction: column;
      width: 300px;
      gap: 10px;
      background-color: #ffffff;
      padding: 20px;
      border-radius: 10px;
      box-shadow: 0 0 10px rgba(0,0,0,0.1);
    }

    form#loanForm input,
    form#loanForm button {
      padding: 8px;
      font-size: 14px;
      border: 1px solid #ccc;
      border-radius: 4px;
    }

    form#loanForm button {
      background-color: #007bff;
      color: white;
      border: none;
      cursor: pointer;
    }

    form#loanForm button:hover {
      background-color: #0056b3;
    }
  </style>
</head>
<body>
  <!-- Logo Kemnaker -->
   <div class="logo-row">
    <img src="CTm_g-pz_400x400-removebg-preview.png" alt="Logo Kemnaker" class="logo-kemnaker">
    <img src="tikbbpvp.png" alt="Logo BBPVP" class="logo-tik">
  </div>

<h1>Peminjaman Barang Inventaris</h1>

  <form id="loanForm">
    <input type="text" id="borrower" placeholder="Nama Peminjam" required />
    <input type="text id="itemId" placeholder="NIP/NIK" required />
    <input type="txt id" id="itemCode" placeholder="Kode Barang" required />
    <input type="number" id="quantity" placeholder="Jumlah" required />
    <p>Tanggal Peminjaman:</p>
    <input type="date" id="loanDate" required />
     <p>Tanggal Pengembalian:</p>
    <input type="date" id="returnDate" required />
    <button type="submit">Pinjam</button>
     <p class="info">*Untuk Pegawai Kemnaker, gunakan NIP. Untuk Pegawai Non-Kemnaker, gunakan NIK.</p>
  </form>

  <script src="js/main.js"></script>
  <br>
</body>
</html>
