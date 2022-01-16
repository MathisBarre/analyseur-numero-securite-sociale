# Analyseur de numéro de sécurité social français

## API

Il suffit de donner le numéro de sécurité sociale complet à la fonction ssnparser (ssn pour Social Security Number) pour que celle-ci le valide et retourne les informations utiles contenu dedans.

```js
import ssnparser from "ssnparser"

const { gender, birth, frenchDepartment } = ssnparser(294037512000522)

console.log(gender) // => "woman" (or "man")
console.log(birthdate) // => {  raw : { month: 03, partialYear: 94 }, predicted: { completedYear: 1994, completeBirthdate: "03-1994" } }
console.log(frenchDepartment) // => 75
```