# react-native-localstorage
None async local storage

## [Installation]
    npm install --save react-native-sync-localstorage

## [Usage]

### 1. Loading stored values at beginnig
    import localStorage from 'react-native-sync-localstorage'

    ...

    localStorage.getAllFromLocalStorage()
      .then(() => {
        // Do Something after loading...
      })
      .catch(err => {
        console.warn(err)
      })

### 2. Use local storage comfortable
#### 2-1. Setting
    const value = 12345
    localStorage.setItem('key', value)

#### 2-2. Getting
    localStorage.getItem('key')

#### 2-3. Deleting
    localStorage.removeItem('key')