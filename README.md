# Package_learnig 
`/// bash`
#LODASH 
lodash est une libraie qui ajoute des methodes sur types de donnée de js

#*installion 

   apres telechargement sur le site officiel
            
            <script src="lodash.js"></script>
   ou en utilisant le cdn
   
#*utilisation 

lodash utilise un objet undescore _
a travers lequel on a accès a differentes méthodes

Exemple :
            
           var demo = " chaine "
          _.trim(demo)
          affiche chaine sans les espaces au debut et a la fin
          
          
Exemple : 
           
           var demo = [1,2,3]
           console.log(_.sample(demo))
           affiche un nombre aleatoire dans le tableau


#bower 
  bower un gestionnaire de paquet coté client 
  #*installtion
  
        npm install -g bower
  
  #*utilisation 
  
      bower install <package>
  
  exemple : 
         
         bower install jquery
  
  pour utiliser le package installer il faut aller dans le dossier bower-components/nom_du_package/dist/le_fichier
  
  exemple :
         
         <script src="bower_components/jquery/dist/jquery.min.js"></script>
  
  
  #multer 
    multer est un module nodejs qui permet de traiter les formulaires contenant les fichiers
    
   #*installation 
   
      npm install multer --save
   
   #*utilisation
   
      const multer = require('multer')
      const upload = multer({disk:'upload/'}) 
      // {disk:'upload/'}créer un dossier a la racine du dossier pour stocker le filename
      du fichier uploader
   
   exemple
   
      app.post('/post',unpload.single('nomdufichierdansleformulaire'),(req,res)=>{
      req.file stock les infos sur le fichier
      req.body stock les champs du formulaire
      })

   #axios 
   axios une librarie javascript qui permet de faire des requetes http asyncchrone elle dispose ddes methodes tel que get ou post
   
   
   #*installation
   
   par la ligne de commande
   
        npm install axios
        bower install axios
   par cdn :
   
        <script src="https://unpkg.com/axios/dist/axios.min.js"></script>
        
   #*utilisation coté client
    
     <form>
     <input type="text"id="nom">
     </form>
     const nom = document.querySelector('#nom')
     const url = '/'
     let mesDonnes = new FormData()
     mesDonnes.set('nom',nom.value)
      axios.post({
      method:post,
      url:url,
      data:mesDonnes
      })
      .then(response){
      console.log(response)
      }
      .catch(){
      console.log('erreur')
      }

    
 #vanillaJS
   
`/// bash`
