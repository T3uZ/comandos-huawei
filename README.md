# Listar interfaces e visualizar suas descrições

```
display interface description
```
![image](https://github.com/user-attachments/assets/3948a189-6684-4fc5-b3b6-6960cf82834a)

- *VLANIF* normalmente relacionado a MPLS.

![image](https://github.com/user-attachments/assets/53a228d8-9c2e-4e00-9769-8bca6d744359)

- *XGigabitEthernet 0/0/18* Interface fisica do equipamento, fibras conectada diretamente.

# Verificar sinal da interface/fibra

```
display transceiver diagnosis interface XGigabitEthernet 0/0/18
```

- Verificar o campo ( RxPower(dBm)    -6.40  ), EX.: Sinal tá sendo -6.40dBm.

# Verificar status da interface
```
display interface XGigabitEthernet 0/0/1
```
-*Last physical down time* mostra o horario da queda.

![image](https://github.com/user-attachments/assets/92caf266-c5aa-4cda-99e0-7f1e564a63ef)


# Verificar modelo de gbic

- Transceiver Type               :10GBASE_LR_SFP (Verificar capacidade do GBIC)
- Wavelength(nm)                 :1270           (Verificar frequencia)
- Transfer Distance(m)           :80000(9um)     (Verificar quantos GBIC)

![image](https://github.com/user-attachments/assets/96da0c40-735e-4b1d-b0d1-10fdaea530a7)
