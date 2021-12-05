# webforce3-bases-jee

### Exercices 1

Créer un petit formulaire qui demande le nom d'un utilisateur et le retourne

#### Étape 1 Créer un projet JEE

    Aller sur File -> New -> Dynamic Web Project-> Entrez le nom que vous souhaitez donner à votre projet 
    
    -> Choisissez le serveur ou installez-le ...



#### Étape 1 Créer un fichier input.html

Fichier input.html à créer dans src/main/webapp



     <!DOCTYPE html>
    <html>
    <head>
    <meta charset="UTF-8">
    <title>Demo servlet avec username input</title>
    </head>
    <body>
    <form method="get" action="HelloServlet">
    <pre>
      Entrez votre nom: <input type="text" name=t1>

       <input type=submit> <input type=reset>
     </pre>
     </form>
     </body>
      </html>

#### Étape 2 Créer un servlet HelloServlet dans src/main/java

Code à remplir dans la méthode doGet() pour le traitement du fichier


      PrintWriter pw = response.getWriter();
		String s = request.getParameter("t1");
		pw.println("<h1>Bonjour," + s);
		pw.close();
		
		
		
#### Étape 3 Si vous avez votre serveur Tomcat, faites un click droit sur input.html puis cliquer Run as -> Run on server




          
          
          
