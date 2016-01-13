# tips

## “Darkleech iframes”  in wordpress : detection and removal

If antivirus detect your website like dangerous with the following alerts
- Infection JS:Injection-A [Trj]
- Web Attack: Mass Injection Website 19

Search in your website folder one of theses elements
- ```grep -r "istart" .```
- ```grep -r "passssword" .```

If match, edit the file with wim and apply this command
```
:%s#//istart\_.*iend##g
```
