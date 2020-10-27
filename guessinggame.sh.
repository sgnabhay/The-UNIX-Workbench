#!/usr/bin/env bash
# File: guessinggame.sh

function guessloop {
  while [[ $response -ne $correct_number ]]
  do 
    if [[ $response -lt $correct_number ]]
    then
      echo "Your guess is too low. Please enter a number again:"
      read response
    elif [[ $response -gt correct_number ]]
    then
      echo "Your guess is too high. Please enter a number again:"
      read response
    fi
  done
  echo "Congratulations! Your answer is correct!"
}

echo "Plese enter how many files are in the current directory:"
read response
correct_number=$(ls | wc -l)
guessloop response correct_number
