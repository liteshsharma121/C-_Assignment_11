
#include <iostream>
#include <list>
#include <vector>
#include <algorithm>
using namespace std;

int main() {
    // LIST CONTAINER
    list<int> l = {12, 25, 8, 40};

    cout << "LIST CONTAINER" << endl;

    cout << "Initial List: ";
    for (int x : l)
        cout << x << " ";
    cout << endl;

    l.push_front(5);
    l.push_back(60);

    cout << "After Insertion: ";
    for (int x : l)
        cout << x << " ";
    cout << endl;

    l.remove(25);

    cout << "After Deletion: ";
    for (int x : l)
        cout << x << " ";
    cout << endl;

    l.sort();

    cout << "Sorted List: ";
    for (int x : l)
        cout << x << " ";
    cout << endl;

    cout << "List Size: " << l.size() << endl;

    // VECTOR CONTAINER
    vector<int> v = {45, 15, 35, 5};

    cout << "\nVECTOR CONTAINER" << endl;

    cout << "Initial Vector: ";
    for (int x : v)
        cout << x << " ";
    cout << endl;

    v.insert(v.begin() + 2, 25);
    v.push_back(55);

    cout << "After Insertion: ";
    for (int x : v)
        cout << x << " ";
    cout << endl;

    v.erase(v.begin() + 1);

    cout << "After Deletion: ";
    for (int x : v)
        cout << x << " ";
    cout << endl;

    sort(v.begin(), v.end());

    cout << "Sorted Vector: ";
    for (int x : v)
        cout << x << " ";
    cout << endl;

    cout << "Vector Size: " << v.size() << endl;

    return 0;
}
