function getFirstDayOfWeek(date) {
    if (!date) date = new Date();
    var day = date.getDay() || 7;
    const dd = new Date(date.getFullYear(), date.getMonth(), date.getDate() + 1 - day);
    const dd2 = new Date(date.getFullYear(), date.getMonth(), date.getDate() + 1 - day + 5);
    return (dd.getMonth() + 1) + "/" + dd.getDate() + "-" + (dd2.getMonth() + 1) + "/" + dd2.getDate();
};
test1

this is change in master