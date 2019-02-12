# Vaja4-interrupt-button-STM32F0

#ODGOVORI

2. b) digitalni vhod kot interrupt (GPIO_EXT...): PA0
      izhod za zeleno LED: PC9

3. c) HAL_GPIO_TogglePin(GPIOC, GPIO_PIN_9);
	    for(uint32_t i=0; i<10000; i++);
   d) 50ms
   e) HAL_GPIO_TogglePin(GPIOC,GPIO_PIN_8);
	 f) HAL_Delay(500);
   
4. b) Modra LED dioda utripa konstantno. Ko pritisnemo modro tipko se prižge oz. ugasne zelena LED dioda.
   c) Pritisk modre tipke ne vpliva na modro LED diodo, zato ker je koda za modro LED diodo zapisana v svoji zanki in ne v tisti kjer           uporabljamo modro tipko.

#KOMENTAR

Program deluje tako, da modra LED dioda konstantno utripa neglede na uporabo modre tipke. Ko pritisnemo modro tipko, se prižge oz. ugasne zelena LED dioda. Program deluje brezhibno.
