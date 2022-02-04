## Object-Crud-doc

### Add property to an Object:

     var brooklynNineNine = {
            name: 'Raymond Holt',
            currentRole: 'Captian of brooklyn99',
          }
          
          brooklynNineNine.husband = 'Kevin' 
          
          // Or brooklynNineNine['husband'] = 'Kevin'

          console.log(brooklynNineNine)
          
  
  ### ES7 Syntax Add property
  
        var list =
          {
            name: 'Michael Scott',
            company: 'Dunder Mufflin',
            designation: 'Regional Manager',
            show: 'The Office',
          },


          new_obj = { ...list, partner: 'Holly Flax' }

          console.table(new_obj)
          
          
 ## Delete property from an Object:
 
           var brooklynNineNine = {
           
            name: 'Amy Santiago',
            currentRole: 'Detective brooklyn99',
            husband: 'Jake Peralta',
            mentor: 'Raymond Holt'
            
          }

          delete  brooklynNineNine.mentor;

          console.log(brooklynNineNine)
          
  ## Update the value of the existing property:
  
             var favChar = {
                name: 'Michael Scott',
                company: 'Dunder Mufflin',
                designation: 'Regional Manager',
                show: 'The Office'
             }

            favChar.designation = 'Hero of Threat Level Midnight'

            console.table(favChar)
            
  ## Add the properties to the array of Object:
  
             
             
             const list = [
                {
                  name: 'Michael Scott',
                  company: 'Dunder Mufflin',
                  designation: 'Regional Manager',
                  show: 'The Office'
                },
                {
                  name: 'Barney Stinson',
                  company: 'Golaith National Bank',
                  designation: 'Please',
                  show: 'How I met your mother'
                },
                
              ]

              list.forEach(function (element) {
                element.favCharacter = "true";
              });

              console.table(list)

 
 
 
 ### Update every values of the existing property in the array of Objects:
 
        const list = [
              {
                name: 'Michael Scott',
                company: 'Dunder Mufflin',
                designation: 'Regional Manager',
                show: 'The Office',
                responsibility: 'heart of the show'
              },
              {
                name: 'Barney Stinson',
                company: 'Golaith National Bank',
                designation: 'Please',
                show: 'How I met your mother',
                responsibility: 'heart of the show'

              },

            ]

            list.every(element => element.responsibility = 'making people laugh') // every method is used to iterate through the array


            console.table(list)



