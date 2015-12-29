# yukimei
var createPet = function () {
	var sex;
	return {
		a : 1,
		setName : function(newName){
			name = newName;
		},
		getName : function(){
			return name;
		},
		getSex : function(){
			return sex;
		},
		setSex : function(newSex){
			if(typeof newSex == 'string' && (newSex.toLowerCase() == 'male' || newSex.toLowerCase() == 'female')){
				sex = newSex;
			}
		}
	}
}
var pet = createPet("vivie");
//console.log(pet.getName());
pet.setName('oliver');
console.log(pet.getName());
pet.setSex("female");
console.log(pet.getSex());
