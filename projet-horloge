var heuresDiv = document.querySelector('.heures');
var dateDiv = document.querySelector('.date');

function affichageHorloge() {
    // Déclaration des variables
    let today, annee, listeMois, mois, jourMois, listeSemaine, jourSemaine, heures, minutes, secondes;

    // Récupérer la date actuelle
    today = new Date();

    // Récupérer l'année
    annee = today.getFullYear();

    // Récupérer le mois
    listeMois = [ "Janvier" , "Février" , "Mars", "Avril" , "Mai" , "Juin" , "Juillet" , "Août" , "Septembre" , "Octobre" , "Novembre" , "Décembre"];
    mois = listeMois[today.getMonth()];

    // Récupérer le jour du mois
    jourMois = today.getDate();

    //Récupérer le jour de la semaine
    listeSemaine = ["Dimanche" , "Lundi" , "Mardi" , "Mercredi" , "Jeudi" , "Vendredi" , "Samedi"];
    jourSemaine = listeSemaine[today.getDay()];

    //Afficher les heures, les minutes et les secondes toujours avec 2 chiffres 
    deuxChiffres = function(e) {
        
        if (e<10) {
            return e = "0" + e;
        }
        else { return e;
        }
    }

    // Récupérer les heures
    heures = deuxChiffres(today.getHours());

    // Récupérer les minutes
    minutes = deuxChiffres(today.getMinutes());

    // Récupérer les secondes
    secondes = deuxChiffres(today.getSecondes());

    //Affichages de l'horloge dans HTML
    heuresDiv.innerText = heures + " : " + minutes + " : "
    dateDiv = jourSemaine + ", " + jourMois + mois + annee;

    //Actualisation toutes les 1s (1000ms)
    setTimeout(affichageHorloge,1000)
}

//Lancer la fonction une fois au début
affichageHorloge();