function gebi(id) {
    return document.getElementById(id);
}

const loadedTDData = localStorage.getItem("TDDATA");
const todos = gebi("todos");

let data = [

]

function ud() {
    localStorage.setItem("TDDATA", JSON.stringify(data));
}

function loadData(arr) {
    todos.innerHTML = "";
    if (arr == null) {
        for (let i = 0; i < data.length; i++) {
            if (data[i].completed) {
                todos.innerHTML += `
                <div>
                    <label class="control control-checkbox">
                        <input type="checkbox" checked="true" onchange="td.setChecked(${i}, this)">
                        <div class="control_indicator"></div>
                    </label><br>
                    <span style="text-decoration: line-through; color: gray;" ondblclick="td.edit(${i}, this)">${data[i].text}</span><br><br>
                    <div class="delete" onclick="td.delete(${i})">&#10005;</div>
                </div><br>
                    `;
            } else {
                todos.innerHTML += `
                <div>
                    <label class="control control-checkbox">
                        <input type="checkbox" onchange="td.setChecked(${i}, this)">
                        <div class="control_indicator"></div>
                    </label><br>
                    <span ondblclick="td.edit(${i}, this)">${data[i].text}</span><br><br>
                    <div class="delete" onclick="td.delete(${i})">&#10005;</div>
                </div><br>
                `;
            }
        }
    } else {
        for (let i = 0; i < arr.length; i++) {
            if (arr[i].completed) {
                todos.innerHTML += `
                <div>
                    <label class="control control-checkbox">
                        <input type="checkbox" checked="true" onchange="td.setChecked(${i}, this)">
                        <div class="control_indicator"></div>
                    </label><br>
                    <span style="text-decoration: line-through; color: gray;" ondblclick="td.edit(${i}, this)">${arr[i].text}</span><br><br>
                    <div class="delete" onclick="td.delete(${i})">&#10005;</div>
                </div><br>
                    `;
            } else {
                todos.innerHTML += `
                <div>
                    <label class="control control-checkbox">
                        <input type="checkbox" onchange="td.setChecked(${i}, this)">
                        <div class="control_indicator"></div>
                    </label><br>
                    <span ondblclick="td.edit(${i}, this)">${arr[i].text}</span><br><br>
                    <div class="delete" onclick="td.delete(${i})">&#10005;</div>
                </div><br>
                `;
            }
        }
    }

    let completedTDS = [];
    for (let i = 0; i < data.length; i++) {
        if (data[i].completed == false) {
            completedTDS.push(data[i]);
        }
    }
    todos.innerHTML += `
    <div class="footer">
        <span class="itemShow">${completedTDS.length} items left</span>
        <span class="link" onclick="td.showAll(this)" id="showAllTd">All</span>
        <span class="link" onclick="td.showActive(this)">Active</span>
        <span class="link" onclick="td.showCompleted(this)">Completed</span>
        <span class="link" onclick="td.clearCompleted()">Clear completed</span>
    </div>`;
}

if (loadedTDData != null) {
    data = JSON.parse(loadedTDData);
    loadData();
} else {
    todos.innerHTML = `
    <div>
        <span>You don't have To-DO's.</span>
    </div>`;
    ud();
}


let lastSec = gebi("showAllTd");

const td = {
    create: (text, completed) => {
        data.push({text: text, completed: completed});
        window.location.href = "index.html";
        ud();
    },

    delete: (todo) => {
        data.splice(todo, 1);
        ud();
        loadData();
    },

    edit: (todo, box) => {
        box.outerHTML = `<input type="text" class="editTodoText" value="${box.innerText}" onchange="td.endEdit(${todo}, this)">`;
    },

    endEdit: (todo, NTBox) => {
        data[todo].text = NTBox.value;
        ud();
        loadData();
    },

    setChecked: (todo, box) => {
        data[todo].completed = box.checked;
        ud();
        loadData();
    },

    showAll: (box) => {
        lastSec.classList.remove("active");
        lastSec = box;
        lastSec.classList.add("active");
        loadData();
    },
    
    showActive: (box) => {
        lastSec.classList.remove("active");
        lastSec = box;
        lastSec.classList.add("active");
        let actives = [];
        for (let i = 0; i < data.length; i++) {
            if (data[i].completed == false) {
                actives.push(data[i]);
            }
        }
        loadData(actives);
    },

    showCompleted: (box) => {
        lastSec.classList.remove("active");
        lastSec = box;
        lastSec.classList.add("active");
        let completed = [];
        for (let i = 0; i < data.length; i++) {
            if (data[i].completed == true) {
                completed.push(data[i]);
            }
        }
        loadData(completed);
    },

    clearCompleted: () => {
        for (let i = 0; i < data.length; i++) {
            if (data[i].completed == true) {
                data.splice(i, 1);
            }
        }
        ud();
        loadData();
    },
}
