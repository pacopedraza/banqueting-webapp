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
      </h3>
    </div>
    <div class="class-history">
      <br />
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
          <br />
    </div>
<div class="class-contacto">
  <div style="text-align:center">
    <h2>Contactanos</h2>
    <p>Será un placer atenderte</p>
    <p>Tel Oficina: 52146138096</p>

  </div>
  <p>
  </p>
  <div class="row">
    <div class="column">
      <img src="../assets/images/mapa_banqueting.jpeg" style="width:100%">
    </div>
    <div class="column">
      <form action="send_email.php">
        <label for="fname">Nombre</label>
        <input type="text" id="fname" name="fname" placeholder="Tú nombre..">
        <label for="tel">Teléfono</label>
        <input type="text" id="tel" name="tel" placeholder="Tu teléfono...">
        <label for="email">Email</label>
        <input type="text" id="email" name="email" placeholder="Tu email...">
        <label for="evento">Evento/Servicio</label>
        <select id="evento" name="evento">
          <option value="boda">Boda</option>
          <option value="xv">XV Años</option>
          <option value="empresarial">Empresarial</option>
          <option value="graduacion">Graduación</option>
          <option value="renta">Renta de mobiliario</option>
        </select>
        <textarea id="subject" name="subject" placeholder="Descripción del servicio..." style="height:170px"></textarea>
        <input type="submit" value="Enviar">
      </form>
    </div>
  </div>
</div>
  </section>
  </body>
</template>

<style scoped>
.class-title {
  background-image: url('https://scontent-sjc3-1.xx.fbcdn.net/v/t31.0-8/892272_485102024882274_1029751940_o.jpg?_nc_cat=104&_nc_oc=AQk7OqBFeqXzjV4HWSJEbvsRXH7Dh7ah9bNxkYV5YJhgGyeSXduYJF9GKOflf3ae8kM&_nc_ht=scontent-sjc3-1.xx&oh=3bc6595b49334797ef5e6b732f5dc77d&oe=5E8B99A9');
  background-repeat: no-repeat;
  background-attachment: fixed;
  background-position: center top;
  
  
  background-size:contain;

  display: flex;
}

h3 {
  color:white;
  text-align: center;
}
html{
    height: 100%
}

* {
  box-sizing: border-box;
}

/* Style inputs */
input[type=text], select, textarea {
  width: 100%;
  padding: 12px;
  border: 1px solid #ccc;
  margin-top: 6px;
  margin-bottom: 16px;
  resize: vertical;
}

input[type=submit] {
  background-color: #4CAF50;
  color: white;
  padding: 12px 20px;
  border: none;
  cursor: pointer;
}

input[type=submit]:hover {
  background-color: #654321;
}

/* Style the container/contact section */
.container {
  border-radius: 5px;
  background-color: #f2f2f2;
  padding: 10px;
}

/* Create two columns that float next to eachother */
.column {
  float: left;
  width: 50%;
  margin-top: 6px;
  padding: 20px;
}

/* Clear floats after the columns */
.row:after {
  content: "";
  display: table;
  clear: both;
}

/* Responsive layout - when the screen is less than 600px wide, make the two columns stack on top of each other instead of next to each other */
@media screen and (max-width: 600px) {
  .column, input[type=submit] {
    width: 100%;
    margin-top: 0;
  }
}

</style>


