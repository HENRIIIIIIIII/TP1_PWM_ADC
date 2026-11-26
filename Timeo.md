## Configuration du timer 1
La valeur de recharge du timer 1 a été calculer avec la formule si dessous :

$$
T_{tick} = \frac{SYSCLK \cdot T_{ms} }{Pre} - 1 = \frac{80\,\text{MHz} \cdot 20 \,\text{ms}}{256} - 1 = 6249
$$

**SYSCLK** : Fréquence de l'horloge du PIC
**Pre** : valeur du prescaler du PIC
**T*ms*** : Fréquence de interruption du timer
**T*tick*** : valeur du registre de reload

J'ai utiliser un prescaler de 256 pour ne pas dépasser la valeur de 16 bits du timer 1.

![enter image description here](Image/Timer1Para.png)

## Configuration du timer 2
La valeur de recharge du timer 1 a été calculer avec la formule si dessous :

$$
T_{tick} = \frac{SYSCLK}{Pre \cdot Freq} - 1 = \frac{80\,\text{MHz}}{16 \cdot 40\,\text{kHz}} - 1 = 124
$$

**SYSCLK** : Fréquence de l'horloge du PIC.

**Pre** : valeur du prescaler du PIC.

**Freq** : Fréquence de interruption du timer.

**T*tick*** : valeur du registre de reload.

J'ai utiliser un prescaler de 256 pour ne pas dépasser la valeur de 16 bits du timer 2.

![enter image description here](/Image/timer2Para.png)
