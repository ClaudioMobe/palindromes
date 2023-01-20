# Palíndromos
Esta función nos dice si la frase que entra como argumento es palíndromo o no :)

  const phrase= 'A man, a plan, a canal: Panama';

  const isPalindrome = (phrase) => {
      //It transforms the string to lower case and replace spaces and non-alphanumerical characters with empty spaces
      let phraseLow=phrase.toLowerCase().replace(/\W/g,'');

      //It transforms the last string to an array so we can reverse the positions and then it is transformed again to a string 
      let phraseLowReversed = phrase.toLowerCase().replace(/\W/g,'').split('').reverse().join('');

      return phraseLowReversed === phraseLow;
  }

  isPalindrome(phrase); //Returns true
