<template>
<body>
  <section class="container">
    <div class="class-title">
      <h3>
        <br />
        <br />
	      <br />
	      <br />
        <br />
	      <br />
	      <br />
        <br />
        <br />
        <br />
        <br />
      </h3>
    </div>
    <div class="class-history">
      <h4>Historia</h4>
      <p>Somos una empresa dedicada al rubro gastronomico y de eventos sociales Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry's standard dummy text ever since the 1500s, when an unknown printer took a galley of type and scrambled it to make a type specimen book. It has survived not only five centuries, but also the leap into electronic typesetting, remaining essentially unchanged. It was popularised in the 1960s with the release of Letraset sheets containing Lorem Ipsum passages, and more recently with desktop publishing software like Aldus PageMaker including versions of Lorem Ipsum.
      </p>
    </div>
    <div class="class-mission">
      <h4>Misi&oacute;n</h4>
      <p>
      Contrary to popular belief, Lorem Ipsum is not simply random text. It has roots in a piece of classical Latin literature from 45 BC, making it over 2000 years old. Richard McClintock, a Latin professor at Hampden-Sydney College in Virginia, looked up one of the more obscure Latin words, consectetur, from a Lorem Ipsum passage, and going through the cites of the word in classical literature, discovered the undoubtable source. Lorem Ipsum comes from sections 1.10.32 and 1.10.33 of "de Finibus Bonorum et Malorum" (The Extremes of Good and Evil) by Cicero, written in 45 BC. This book is a treatise on the theory of ethics, very popular during the Renaissance. The first line of Lorem Ipsum, "Lorem ipsum dolor sit amet..", comes from a line in section 1.10.32.
      </p>
    </div>
    <div class="class-vision">
      <h4>Visi&oacute;n</h4>
      <p>
      Contrary to popular belief, Lorem Ipsum is not simply random text. It has roots in a piece of classical Latin literature from 45 BC, making it over 2000 years old. Richard McClintock, a Latin professor at Hampden-Sydney College in Virginia, looked up one of the more obscure Latin words, consectetur, from a Lorem Ipsum passage, and going through the cites of the word in classical literature, discovered the undoubtable source. Lorem Ipsum comes from sections 1.10.32 and 1.10.33 of "de Finibus Bonorum et Malorum" (The Extremes of Good and Evil) by Cicero, written in 45 BC. This book is a treatise on the theory of ethics, very popular during the Renaissance. The first line of Lorem Ipsum, "Lorem ipsum dolor sit amet..", comes from a line in section 1.10.32.
      </p>
    </div>
        <div class="class-contact">
      <p>Celaya, Guanajuato</p>
      <p>46138096</p>
    </div>
    <div class="class-contacto">
        <form action="/action_page.php">
          <input type="text" id="fname" name="firstname" placeholder="Nombre...">

          <input type="text" placeholder="E-mail..." name="email" required>

          <select id="event" name="event">
            <option value="boda">Boda</option>
            <option value="xvanios">XV Años</option>
            <option value="empresa">Empresarial</option>
            <option value="grad">Graduación</option>
            <option value="otro">Social/Otro</option>
          </select>

           <textarea id="subject" name="subject" placeholder="Cuentamos..." style="height:200px"></textarea>

            <input type="submit" value="Enviar">
          </form>
      </div>
  </section>
  </body>
</template>

<style scoped>
.class-title {
  background-image: url('https://scontent-sjc3-1.xx.fbcdn.net/v/t31.0-8/892272_485102024882274_1029751940_o.jpg?_nc_cat=104&_nc_oc=AQk7OqBFeqXzjV4HWSJEbvsRXH7Dh7ah9bNxkYV5YJhgGyeSXduYJF9GKOflf3ae8kM&_nc_ht=scontent-sjc3-1.xx&oh=3bc6595b49334797ef5e6b732f5dc77d&oe=5E8B99A9');
  background-repeat: no-repeat;
  background-attachment: fixed;
  background-position: right top;
  background-size: auto;
  
  max-width: 100%;
  height: auto;
  width: auto\9;
  
  z-index: 0;
}

h3 {
  color:white;
  text-align: center;
}
html{
    height: 100%
}

body {font-family: Arial, Helvetica, sans-serif;}
* {box-sizing: border-box;}

input[type=text], select, textarea {
  width: 50%;
  padding: 12px;
  border: 1px solid #ccc;
  border-radius: 4px;
  box-sizing: border-box;
  margin-top: 6px;
  margin-bottom: 16px;
  resize: vertical;
}

input[type=submit] {
  background-color: #4CAF50;
  color: white;
  padding: 12px 20px;
  border: none;
  border-radius: 4px;
  cursor: pointer;
}

input[type=submit]:hover {
  background-color: #45a049;
  position: left;
}

.container {
  border-radius: 5px;
  background-color: #f2f2f2;
  padding: 20px;
}

</style>


