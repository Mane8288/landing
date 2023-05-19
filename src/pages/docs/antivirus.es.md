# ¿Por qué mi antivirus dice que Plutonium es un virus?

Plutonium es lo que se conoce como un falso positivo (tu antivirus piensa que Plutonium es un virus, cuando en realidad Plutonium está 100% limpio). Los desarrolladores detrás de este proyecto han estado trabajando en él durante años y se ha dedicado mucho esfuerzo en esto. No arriesgarían toda su credibilidad comprometiendo tu PC con malware.

---

## **¿Por qué está sucediendo esto?**

Plutonium está modificando la memoria de los juegos, al igual que un virus manipularía otros programas, lo que provoca esta detección falsa.

---

## **¿Cómo puedo solucionarlo?** (Windows Defender)

Tenemos un tutorial en video sobre cómo agregar exclusiones a Windows Defender aquí:

<Player url="https://youtu.be/0ijMY8FiLSg" />

Alternativamente, si deseas un método más rápido, puedes ejecutar un comando de PowerShell aquí:
<Details title="Comando de PowerShell para agregar una exclusión en Windows Defender">
La forma más rápida de solucionar esto es hacer clic derecho en el botón de inicio y seleccionar `Windows PowerShell (Administrador)` y luego pegar el siguiente comando:
`powershell -inputformat none -outputformat none -NonInteractive -Command Add-MpPreference -ExclusionPath "%localappdata%\Plutonium"`

Nota: haz clic derecho para pegar.

![GIF que muestra cómo hacerlo](/images/docs/antivirus/Ecyyy6Q.gif)

(Ten en cuenta que esto solo indica a **Windows Defender** que no detecte Plutonium, si tienes otro antivirus, debes consultar su documentación).
</Details>

---

## **¿Cómo puedo solucionarlo?** (Otros antivirus)

Aprende cómo agregar una exclusión de carpeta para Plutonium en tu antivirus específico aquí:
[Malwarebytes](https://support.malwarebytes.com/hc/en-us/articles/360038479234) | [Avast](https://support.avast.com/en-us/article/Antivirus-scan-exclusions/) | [Norton](https://support.norton.com/sp/en/us/home/current/solutions/v3672136) | [Kaspersky](https://support.kaspersky.com/14848#block1)
| [AVG](https://support.avg.com/SupportArticleView?l=en&urlName=AVG-Antivirus-scan-exclusions&supportType=home) | [Bitdefender](https://www.bitdefender.com/consumer/support/answer/13427/) | [ESET NOD32](https://help.eset.com/eav/14/en-US/idh_detection_exclusions.html) | [G Data](https://help.gdatasoftware.com/b2c/GDAV/2014/en/index.html?410057.htm)
[Ahnlab](https://ask.ahnlab.com/hc/en-us/articles/900003233126--V3-ALL-Let-s-learn-about-setting-up-Scan-Exclusions)

Nota: la carpeta que deseas excluir es: `C:\Users\TU-NOMBRE-DE-USUARIO\AppData\Local\Plutonium`

---

### Otras notas

* ***Si estás usando [Web Root](https://community.webroot.com/webroot-secureanywhere-antivirus-12/how-to-uninstall-secureanywhere-317009)/[McAfee](https://service.mcafee.com/webcenter/portal/cp/home/articleview?articleId=TS101331)/[Bullguard](https://www.bullguard.com/support/faq/other/how-do-i-uninstall-bullguard-from-my-computer.aspx)  recomendamos desinstalarlos por completo.***

  * ¿Por qué? Sencillamente, **desactivarlos o permitir exclusiones no permitirá que Plutonium funcione correctamente** (así de malos son esos antivirus).


* Si no puedes encontrar la carpeta "AppData" al intentar agregar una exclusión, tendrás que habilitar las carpetas ocultas. Para hacer esto, abre una nueva ventana del explorador de archivos, haz clic en la pestaña "Ver" y marca la casilla "Elementos ocultos".

![Elementos ocultos](/images/docs/antivirus/EUnBnHg.png)
