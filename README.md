# Kalendar demonstratura

# IDEJA

**Web aplikacija "insert name here" pomaže profesorima, asistentima, laborantima, studentskoj slubži(referadi) i demonstratorima u izvođenju demonstartura.**

* Profesorima[professor] 
    * odobravanje demonstrature putem online obrazca
    * potvrđivanje odrađene demonstrature putem online obrazca
                       
* Asistentima/laborantima[assistant] 
    * organiziranje studenata demonstratora
    * maksimalno pokrivene demonstrature, rasterečenost tijekom viježbe

* Studentima[student]
    * lakša organizacija demonstratura sa slobodnim vremenom
    * optimalno ispunjavanje satnice
                    
* Studentskoj službi[referada] 
    * online prikupljanje prijava
    * online prikupljanje izviješća
                            
### ---------Pred početak semestra---------
### Korak 1
  * Referada otvara poziv za demonstrature - obavijest na home pageu
  * Studentima se šalje mail s linkom
 
### Korak 2
  * Studenti se registriraju - etfos/ferit mail, potencijalno i s AAI
  * Ispunjavaju formu - dohvačanje podataka iz ISVU-a
  * Generira se dokument - šalje se referadi
  
Nakon što se odaberu demonstratori(postupak treba ispitati, možda se može online u ulozi [prodekan],[profesor],[odbor]
### Korak 3
* Studenti su obaviješteni o dobivenoj demonstraturi
  
### ---------Semestar---------
### Korak 4
* Satničar četvrtkom u tjednu X objavljuje raspored za tjedan X+1
###  Korak 5
*  Studnet od četvrtka  16:00 do petka 19:00 ima mogućnost odabrati SVE termine u kojima je slobodan odraditi demonstrature za kolegije[courses] na kojima se nalazi u statusu demonstratora
  
### Korak 6
*  Aplikacija u petak 19:00 generira raspored demonstratora - OPTIMALNO(parametri odrađena satnica, odobrena satnica, mogućnost dolaska i sl)
 * Aplikacija dostavlja mail korisnicima raspored njegovih demonstratura za tjedna X+1
 *  Aplikacija u google kalendar dodaje raspored
  * Aplikacija dostavlja mail asistentima raspored demonstratora za njegov kolegij
  
### Korak 7
 *  Ponavlja se sve od koraka 4
  
### ---------Kraj semestra---------
### Korak 8
  *  Referada postavlja obavijest o podnošenju izvještaja
   
### Korak 9
   * Student ispunjava formu
   
### Korak 10
  *  Profesor potvrđuje formu
   
### Korak 11
 *   Referada zaprima potvrđenu("potpisanu") formu
 
 # Realizacija
  
  ## XAMP
  ##### What is that?
  ##### Instalacija
  
  ## PHPStorm
  ##### What is that?
  * https://www.jetbrains.com/phpstorm/
  ##### Instalacija
   
  ## Laravel
  ##### What is that?
  * PHP web framework 
  * https://laravel.com/
  ##### Instalacija
  * https://laravel.com/docs/4.2
  
 
  ## Algoritam 
  * Korak 6
  
  #### Inputi
1) Laboratorijske vježbe(object list):
*   ime(string),
*   redni broj
*   kolegij
      *   ime
      *   id
*   termini-vježbe(object list)
      *   id
      *   assistent
          *    id
          *    ime
      *   vrijeme početka
      *   vrijeme kraj
      *   demonstratori = NULL
     
2) Raspoloživi studnetski termini(object list):
  *   student
        *   ime
        *   id
        *   odrađen broj sati
        *   odobrene demonstrature
            *   kolegij
                *   id
                *   ime
            *   broj sati
  *   termin vježbe
        *   id
        
   #### Outputi
1) termini-vježbe(object list)
*    id termina vježbe
*    vrijeme početka vježbe
*    vrijeme kraj vježbe
*    demonstratori = student.id
     
  ## Owners
* Nikola Stipić
* Luka Kruljac
  
