<?php

  function post_captcha($user_response){
    $fields_string = '';
    $fields = array(
        'secret' => '6Lc2SSYUAAAAAK6oEAGnBNlP15SEM6bg2i9tbWD5',
        'response' => $user_response
      );
    foreach($fields as $key => $value)
    $fields_string .= $key . '=' .$value . '&';
    $fields_string = rtrim($fields_string, '&');

    $ch = curl_init();
    curl_setopt($ch, CURLOPT_URL, 'https://www.google.com/recaptcha/api/siteverify');
    curl_setopt($ch, CURLOPT_POST, count($fields));
    curl_setopt($ch, CURLOPT_POSTFIELDS, $fields_string);
    curl_setopt($ch, CURLOPT_RETURNTRANSFER, True);

    $result = curl_exec($ch);
    curl_close($ch);

    return json_decode($result, true);
  }

  //Agregamos una variable Captcha
  $res = post_captcha($_POST['g-recaptcha-response']);

  header("Content-type: text/html; charset=\"utf-8\"");
  $error = "";
  $mensajeExito = "";

  if($_POST){
    if($_POST['email'] && filter_var($_POST['email'], FILTER_VALIDATE_EMAIL) === false){
      $error .= "Email no valido.<br/>";
    }
    if ($error != ""){
      $error = '<div class="alert alert-danger" role="alert"><p><b>Se ha producido un error:</b></p>'.$error.'</div>';
    }
    if(!$res['success']){
      $errorCap = '<div class="alert alert-danger" role="alert"><p><strong>Completa el Captcha</strong></p></div>';
    }
    else{
      $nombre = $_POST['nombre'];
      $mail = $_POST['email'];
      $asunto = $_POST['asunto'];
      $mensajeC = $_POST['mensaje'];

      $header = 'From: '.$mail."\r\n";
      $header .= "X-Mailer: PHP/".phpversion()."\r\n";
      $header .= "Mime-Version: 1.0 \r\n";
      $header .= "Content-type: text/plain";

      $mensaje = "Mensaje enviado por ==> " .$nombre.",\r\n";
      $mensaje .= "Utilizando el email ==> ".$mail.".\r\n";
      $mensaje .= "Asunto ==> ".$asunto."\r\n";
      $mensaje .= "Mensaje ==> ".$mensajeC."\r\n";
      $mensaje .= "Enviado el ==> ".date('d/m/Y', time());

      $para = "prestamodispositivos@gmail.com";
      $asunto = "Mensaje desde mi sitio web";

      if(mail($para, $asunto, utf8_decode($mensaje), $header)){
        $mensajeExito = '<div class="alert alert-success" role="alert">Mensaje enviado con exito <3 </div>';
      }
      else{
        $error = '<div class="alert alert-danger" role="alert"><p><strong>Mensaje no enviado</strong></p></div>';
      }
    }
  }
?>

<!DOCTYPE html>
<html lang="en">
  <head>
    <!-- Required meta tags -->
        <title>contacto</title>
    <meta charset="utf-8">
    <meta name="viewport" content="width=device-width, initial-scale=1, shrink-to-fit=no">

    <!-- Bootstrap CSS -->
    <link rel="stylesheet" type="text/css" href="css/bootstrap.min.css">

    <!-- Recaptcha -->
  </head>
  <body>
  
    <!-- Formulario de contacto -->
    <section class="container pt-5 mt-5">
      <h3 class="text-uppercase text-center">formulario de contacto</h3>
      <hr class="hr"/>
      <p class="lead text-center">
        "Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore."
      </p>
      <div><? echo $error.$mensajeExito; ?></div>
      <form action="">
        <div class="row">
          <div class="col-md-6">
            <div class="form-group row">
              <label for="nombre" class="col-md-2 col-form-label">Nombre:</label>
              <input type="text" class="form-control col-md-10" placeholder="Ingrese su nombre"
              id="nombre" name="nombre">
            </div>
            <div class="form-group row">
              <label for="email" class="col-2 col-form-label">Email:</label>
              <input type="email" class="form-control col-md-10" placeholder="Ingrese su email"
              id="email" name="email">
            </div>
            <div class="form-group row">
              <label for="asunto" class="col-md-2 col-form-label">Asunto:</label>
              <input type="text" class="form-control col-md-10" placeholder="Ingrese el asunto" id="asunto" name="asunto">
            </div>
          </div>
          <div class="col-sm-12 col-md-6">
            <div class="form-group" style="height: 20vh;">
              <textarea class="form-control h-100 d-inline-block" placeholder="ingrese su mensaje" id="mensaje" name="mensaje"></textarea>
            </div>
          </div>
        </div>
        <div class="form-group row d-flex justify-content-center">
          <button class="btn btn-primary col-md-6" type="submit">Enviar</button>
        </div> 
        <div><? echo $errorCap; ?></div>
        <div class="form-group row">
          <div class="g-recaptcha offset-md-2 col-sm-5" data-sitekey="6Lc2SSYUAAAAAHFz_Xb2HsrTr98SHoF2UXaw_gC4"></div>
        </div>
      </form>
    </section>
    <!-- Fin formulario de contacto-->
    

    <hr class="hr">
    <hr class="hr">


    <!-- jQuery first, then Tether, then Bootstrap JS. -->
    <script src="https://code.jquery.com/jquery-3.1.1.slim.min.js" integrity="sha384-A7FZj7v+d/sdmMqp/nOQwliLvUsJfDHW+k9Omg/a/EheAdgtzNs3hpfag6Ed950n" crossorigin="anonymous"></script>
    <script src="https://cdnjs.cloudflare.com/ajax/libs/tether/1.4.0/js/tether.min.js" integrity="sha384-DztdAPBWPRXSA/3eYEEUWrWCy7G5KFbe8fFjk5JAIxUYHKkDx6Qin1DkWx51bBrb" crossorigin="anonymous"></script>
   <script type="text/javascript" src="js/bootstrap.min.js"></script>
  </body>
</html>
