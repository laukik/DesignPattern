Bridge Design Pattern
-------------------------------
It decouples an abstraction from its implementaion so that they can behave indipendently.
//We apply Adaptor when we need to make two contracts compitable, But we apply Bridge
//So that we don't need to face the issue..


interface IAbstarction{
    IImplmentor implementor;
}

class Abstarction implements IAbstarction{
    
}

interface IImplmentor{
    
}

interface Implmentor implements IImplmentor{
    IImplmentor implementor = concreteImplementor;
}