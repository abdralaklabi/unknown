# unknown
I don't know 
const howOld = (age, year) => {
  let real = year;
  year -= 2020;
  let agepast =  age + year;
  let before = Math.abs(agepast);
  if (year > 0) {
  return `You will be ${age + year} in the year ${real}`; 
  } else if (year < 0 && 0 > agepast) {
    return `The year ${real} was ${before} years before you were born`
  } else if (year < 0 && 0 < agepast) {
    return `You were ${agepast} in the year ${real}`
  } else if (0 === agepast) {
    return `you were born in ${real}`
}};
console.log(howOld(20, 1999))
