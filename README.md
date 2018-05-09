# Instruktioner

OBS: Denna guide är anpassad efter Windows 7 32-bitars.

Först och främst så måste du aktivera Ctrl + Alt + Delete i SEB.

Gå till: 

Windows Menyn -> "Safe Exam Browser" -> "SEB Config Tool".

Gå sedan till Registry och Ticka alla alternativ; detta kommer se till så att Ctrl Alt Delete fungerar som det ska.
Tryck på File -> Save Settings. 

- Och du ska kunna använda Ctrl Alt Delete när du är i SEB, nu. Det enda problemet är bara att det inte finns några knappar förutom "avbryt". Vi vill kunna byta användare och ha på SEB i bakgrunden så att pogrammet tror att vi fortfarande sitter där.

Nu så behöver du ett konto du kan byta till, om du är administratör på din dator så är det lätt att fixa.

Öppna och kör cmd.exe som administratör

Skriv in "net user"; finns det ett konto som heter Administrator eller liknande så är det bara att ändra lösenord på den genom att skriva "net user Administrator*" och sedan "ditt" nya lösenord två gånger. 

De flesta datorer kräver att du har ett lösenord längre än 8 tecken, minst en versal (stor bokstav), minst ett nummer, och minst en gemen (Liten bokstav). Möter du inte dessa krav så kommer du inte kunna logga in.

När allt det är fixat, se till att logga in på Administrator så att du slipper vänta på "first time setup" eller liknande då du väl byter användare.

# Om du INTE har ett adminkonto:

Gå till Kontrollpanelen\Användarkonton\Användarkonton -> Hantera Användarkonton och skapa en admin-användare.

# Innan du startar SEB

1. Kör programmet (det här) som Administratör. Filen finns tillgänglig som SetSwitchKey.exe

2. Ha på det i bakgrunden då SEB körs.

Detta kommer förhindra SEB att ändra registernyckeln på HideFastUserSwitching, det vill säga "Växla Användare". Detta kommer låta dig byta användare. Programmet kommer även aktivera KeepRasConnections, vilket innebär att du inte kan bli bortkopplad från internet då du byter användare.

Och nu kan du byta användare hur du vill.
