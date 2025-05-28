# homewor-20.05
//задание 1

const daysOfWeek = {
    1: "Понедельник",
    2: "Вторник",
    3: "Среда",
    4: "Четверг",
    5: "Пятница",
    6: "Суббота",
    7: "Воскресенье"
};
console.log(daysOfWeek[2]);
const user = {
    name: "Денис",
    surname: "Лобов",
    age: 17
};
console.log(`${user.surname}-${user.name}-${user.age}`);
user.patronymic = prompt("Наипиште ваше отчество:");
delete user.surname;

//задание 2
const arr1 = ['пн', 'вт', 'ср', 'чт', 'пт', 'сб', 'вс'];
const arr2 = [1, 2, 3, 4, 5, 6, 7];
const weekDays = {};
for (let i = 0; i < arr1.length; i++) {
    weekDays[arr1[i]] = arr2[i];
}
console.log(weekDays);
const obj = {x: 1, y: 2, z: 3};
for (let key in obj) {
    obj[key] = obj[key] ** 2;
}
console.log(obj);

//заданеи 3

const obj = { 
    key1: { 
        key1: 1, 
        key2: 2, 
        key3: 3, 
    }, 
    key2: { 
        key1: 4, 
        key2: 5, 
        key3: 6, 
    }, 
    key3: { 
        key1: 7, 
        key2: 8, 
        key3: 9, 
    }, 
};
for (let key in obj) {
    for (let innerKey in obj[key]) {
        sum += obj[key][innerKey];
    }
}
console.log(sum);
