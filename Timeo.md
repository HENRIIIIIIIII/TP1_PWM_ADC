## Configuration du timer 1
La valeur de recharge du timer 1 a été calculer avec la formule si dessous :

$$
T_{tick} = \frac{SYSCLK}{Pre \cdot Freq} - 1 = \frac{80\,\text{MHz}}{256 \cdot 10\,\text{Hz}} - 1 = 31249
$$

SYSCLK : Fréquence de l'horloge du PIC
Pre : valeur du prescaler du PIC
Freq : Fréquence de interruption du timer
T*tick* : valeur du registre de reload

J'ai utiliser un prescaler de 256 pour ne pas dépasser la valeur de 16 bits du timer 1.
