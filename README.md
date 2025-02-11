[read_file for 'script.js'] Result:

const buttonNo = document.querySelector('#no')
const buttonYes = document.querySelector('#yes')

let fontSize = 2

let messages = [
  'Estas segura?',
  'De verdad estas segura?',
  'segurisima segurisisisma?',
  'de verdad?',
  'andale dime q si'
]

buttonNo.addEventListener('click', () => {
  fontSize = fontSize + .5
  buttonYes.style.fontSize = `${fontSize}rem`

  const indexRandom = Math.floor(Math.random() * messages.length)

  buttonNo.textContent = messages[indexRandom]
})

buttonYes.addEventListener('click', () => {
  document.querySelector('#message').style.display = 'flex'
})

<environment_details>
# VSCode Visible Files
README.md

# VSCode Open Tabs
index.html
style.css
README.md
script.js
</environment_details>
