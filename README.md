# micro-drum
Contexte : dans cette expérience, on enregistre l'angle d'avalanche de 4 micro-tambours tournant dans le sens anti-horaire. 
L'objectif de ce programme est de calculer cet angle pour une série d'images, et que les valeurs soient enregistrées dans des tableaux type df (ou array de df), 
chaque tableau correspondant aux valeurs d'un microtambour de l'expérience. 
Pour réaliser les tests, 5 images successives d'une expérience sont fournies.   
Le programme doit pouvoir identifier les 4 tambours pour chaque image (= 4 cercles/image). 
Ensuite il doit calculer l'angle d'avalanche (=pente) dans chaque cercle défini (code déjà écrit, fait via transformée de Hough).
Les valeurs des angles doivent être sauvegardées dans des tableaux type df avec les colonnes suivantes : ["av_angle_T1"], ["std_T1]. (T1 = micro-tambour n°1).
Pour que le programme puisse "reconnaître" chaque tambour, il faut calculer la distance minimale entre chaque tambour d'une image n à l'image n+1 (fonction en cours).
