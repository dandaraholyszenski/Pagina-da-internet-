!DOCT<!DOCTYPE html>
<html lang="pt-br">
<head>
   <meta charset="UTF-8">
   <meta name="viewport" content="width=device-width, initial-scale=1.0">
   <title>Blog do palmeiras</title>


   <style>
       body{
           margin: 0;
           font-family: Arial, Helvetica, sans-serif;
           background-color: #f4f4f4;
       }


       header{
           background-color: #00a11b;
           color: white;
           text-align: center;
           max-width: 800px;
           margin: 20px auto 0;
           padding: 20px;
       }


       main{
           background-color: white;
           max-width: 800px;
           margin: 0 auto;
           padding: 20px;
           display: flex;
           gap: 20px;
           align-items: center;
           box-shadow: 0 0 10px rgba(102, 7, 7, 0.2);
       }


       img{
           width: 180px;
           height: 180px;
           object-fit: cover;
           border-radius: 10px;
       }


       h2{
           color: #08e625;
       }


       p{
           color: #080808;
       }
   </style>
</head>


<body>


<header>
   <h1>Blog do Palmeiras</h1>
   <p>Curiosidades e noticias da Sociedade Esportiva Palmeiras.</p>
</header>


<main>
   <img src="images.jpeg"
        alt=palmeiras">


   <div>
       <h2>Primeiro Post</h2>


       <p><strong>Por:</strong> Dandara Luiza</p>


       <p>
        sociedade Esportiva Palmeiras foi fundado em 1914 como Palestra Italia e adotou o nome Palmeiras em 1942.
        É um dos clubes mais vitoriosos do Brasil, com títulos importantes como o Campeonato Brasileiro Série A e a Copa Libertadores da América.
        Atualmente, joga no Allianz Parque e é reconhecido por sua tradição, torcida e sucesso no futebol nacional e internacional
        
       </p>
   </div>
</main>


</body>
</html>
<button onclick="curtir()">
   ❤️ <span id="likes">0</span>
</button>
<button onclick="gostar()">
   👎​​ <span id="gostei">0</span>
</button>
<script>
   let likes = 0;
   let gostei = 0;
   let curtiu = false;
   let gostou = false;
   function curtir() {
       if (curtiu) {
           likes--;
           curtiu = false;
       } else {
           likes++;
           curtiu = true;
       }
       document.getElementById("likes").textContent = likes;
   }
   function gostar() {
       if (gostou) {
           gostei--;
           gostou = false;
       } else {
           gostei++;
           gostou = true;
       }
       document.getElementById("gostei").textContent = gostei;
   }
</script>
